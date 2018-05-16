<template>
  <div>
    <div class=form-group>
      <form>
        <table>
          <tr>
            <td>
              <label>Name</label>
              <td><input type=text v-model='names'></td>
          </tr>
          <tr>
            <td>
              <label>Email</label>
              <td><input type=email v-model='email'></td>
          </tr>
          <tr>
            <td>
              <label>Mobile Number</label>
              <td><input type=number v-model='num'></td>
          </tr>
        </table>
      </form>
    </div>
    <component2 :feild1='names' :feild2='email' :feild3='num'></component2>
  </div>

</template>

<script>
import component2 from '@/components/component2';

export default {
  name: 'HelloWorld',
  components: {
    component2,
  },
  data() {
    return {
      names: '',
      email: '',
      num: '',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.form-group {
  text-align: center;
  margin-left: 35%;
}
.form-group table td {
  padding-top: 20px;
  padding-left: 15px;
}
.form-group table input {
  font-size: 20px;
  height: 30px;
  width: 80%;
}
</style>
