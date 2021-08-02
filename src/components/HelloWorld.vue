
<template>

  <div class="row">
    <a href="https://s2mworldwide.com/" class="link-success">
    <div class="TexteLien" >
    <h1>ITSP Parameters Management Rest APIs</h1>
    
  </div>
  </a>
  </div>
  
  <div class="row">
  <div id="app" v-for="item in data.tags" :key="item">
    <a href="#" class="link-success">
    <div class="col">
         <h1>{{item.name}}</h1>
         {{item.description}}
         </div>
    </a>
     </div>
  </div>

</template>

<script>
import apiData from "./api.json";

export default {
  data() {
    return {
      data: apiData,
    };

  },
};
</script>
<style>
.col {
  float: left;
  width: 40%;
  height: 110px;
  margin-right: 50px;
  margin-left: 60px;
  margin-top: 25px;
  box-shadow: 8px 8px 15px #00000038;
  background-color: white;
  border-radius: 10px;
}
.column {
  float: left;
  width: 60%;
  height: 110px;
  margin-right: 50px;
  margin-left: 250px;
  margin-top: 25px;
  box-shadow: 8px 8px 15px #00000038;
  background-color: white;
  border-radius: 10px;
}
.col:hover
{
background-color: #ecb8c4;
}
/* Clear floats after the columns */
.row:after {
  content: "";
  display: flex;
  clear: both;
}

body {
  background-color: #f7f7f7;
}

div.TexteLien
{
background-color: white;
  float: left;
  width: 60%;
  height: 110px;
  margin-right: 50px;
  margin-left: 250px;
  margin-top: 25px;
  box-shadow: 8px 8px 15px #00000038;
  background-color: white;
  border-radius: 10px;
}

div.TexteLien:hover
{
background-color: #ecb8c4;
}


</style>
