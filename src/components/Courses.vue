<template>
  <h1> Sustainable Watering plan</h1> 
   <div class="container">
      <table id="demo-table-id" class="table table-striped">
        <caption></caption>
        <thead>
          <tr>
            <th>Hole</th>
            <th>Fairway </th>
            <th>Greens</th>
            <th>Teebox</th>
            <th>Roughs</th>
          </tr>
        </thead>
        <tbody>
         <tr>
            <td><input type="checkbox" id="checkbox" v-model="checked">
            <label for="checkbox">{{ checked }}</label>- Disable if it WILL rain</td>
            <td><button type="button" class="btn btn-primary"> minute</button> </td>
            <td><button type="button" class="btn btn-success">  minutes</button> </td>
            <td><button type="button" class="btn btn-info">  minutes</button> </td>
            <td><button type="button" class="btn btn-info">  minutes</button> </td>
          </tr>
          <tr>
            <td>1  </td>
            <td> 10</td>
            <td>13</td>
            <td>8</td>
            <td>12</td>
          </tr>
          <tr>
            <td>2 </td>
            <td> 9</td>
            <td>13</td>
            <td>15</td>
            <td>12</td>
          </tr>
          <tr>
            <td>3 </td>
            <td> 12</td>
            <td>13</td>
            <td>8</td>
            <td>12</td>
          </tr>
          <tr>
            <td>4</td>
            <td> 10</td>
            <td>13</td>
            <td>15</td>
            <td>12</td>
          </tr>

          <tr>
            <td>5 </td>
            <td> 10</td>
            <td>10</td>
            <td>15</td>
            <td>12</td>
          </tr>
          <tr>
            <td>6 </td>
            <td> 10</td>
            <td>15</td>
            <td>8</td>
            <td>15</td>
          </tr>
          <tr>
            <td>7 </td>
            <td> 10</td>
            <td>15</td>
            <td>15</td>
            <td>12</td>
          </tr>
          <tr>
            <td>8 </td>
            <td> 11</td>
            <td>15</td>
            <td>15</td>
            <td>12</td>
          </tr>
          <tr>
            <td>9 </td>
            <td> 8</td>
            <td>15</td>
            <td>15</td>
            <td>12</td>
          </tr>
          <tr class="info">
            <td colspan="4"></td>
            <td>
              <b>1173</b>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
</template>

<script>
 import axios from "axios";

 export default {
  name: "Courses",
  data () {
    return {
        courses: null,
    };
  },
  created: function() {
      axios
        .get("https://mocki.io/v1/69bd11f5-7c1d-4637-8a20-07acbd823cf1")
        .then (res => { this.courses = res.data;});
  }
};
</script>

<style>
   h1 {margin-bottom:5%}
</style>
