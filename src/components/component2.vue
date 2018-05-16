<template>

  <div>
      <div class="display">
        <table>
          <tr>
            <td>Name :</td>
            <td><p>{{feild1}}</p></td>
          </tr>
          <tr>
            <td>E-Mail :</td>
            <td><p>{{feild2}}</p></td>
          </tr>
          <tr>
            <td>Mobile Number :</td>
            <td><p>{{feild3}}</p></td>
          </tr>
        </table>
      </div>
  </div>
</template>

<script>
export default {
  props: ['feild1', 'feild2', 'feild3'],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.display{
    margin-left:35%;
    margin-top: 2%;
}

.display table tr,td{

           padding-left: 10px;
           padding-right: 40px;
           padding-top: 40px;
}

</style>
