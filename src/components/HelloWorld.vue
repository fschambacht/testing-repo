<template>
  <div class="hello">
    <form
      id="paymentForm"
      action="https://www.bridgepaynetsecuretest.com/WebSecurity/echo.aspx"
      method="post"
      style="margin: 10px"
    >
      <select
        class="form-control"
        name="amount"
        id="amount"
        style="width: 100px"
      >
        <option value="25">$25</option>
        <option value="50">$50</option>
      </select>
      <div
        class="preserveHtml"
        id="card"
        style="
          border: solid 1px lightgray;
          height: 100px;
          width: 500px;
          padding: 20px 10px;
          border-radius: 10px;
          margin: 10px 0px;
        "
      ></div>
      <div
        class="preserveHtml"
        id="errorMessage"
        style="margin-bottom: 10px; color: #c0392b"
      ></div>
      <button type="submit" class="btn btn-default">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  created() {
    console.log("created");
  },
  methods: {
    tokenPay() {
      console.log("token pay");
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
