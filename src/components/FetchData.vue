<script>
import axios from "axios";
export default {
  name: "FetchData",
  props: ['url'],
  data() {
    return {
      response: null,
      loading: true,
    }
  },
  created() {
    axios.get(this.url)
        .then(response => {
          this.response = response.data;
          this.loading = false;
        })
        .catch(error => {
          console.log(error + '에러입니다.');
        })
  },
  render() {
   return this.$scopedSlots.default({
     response: this.response,
     loading: this.loading
   })
  }
}
</script>
