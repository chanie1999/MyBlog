<template>
  <div class="Introduction">
    <div class="side">
      <div class="intr-img">
          <img src="../assets/header.jpg" alt="龙雨">
        <lable>Chanie's BLOG</lable>
        <table>
          <tr>
            <th>liked</th>
            <th>blog</th>
            <th>visited</th>
          </tr>
          <tr>
            <td>0</td>
            <td>0</td>
            <td>0</td>
          </tr>
        </table>
        <p style="font-size:20px;
                  font-family:微软雅黑;
        ">life is just like the sea,only the strong will can come over it.</p>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    name: "Introduction"
  }
</script>

<style scoped>
.side{
  width: 350px;
  height: 500px;
  background: rgba(119,136,153,0.2);
  position: absolute;
  margin: 50px 35px auto;
  border-radius: 5px;
}
.intr-img{
  margin: 40px auto;
  text-align: center;
  width: 170px;
  height: 170px;
  }
img{
  width: 120px;
  height: 120px;
  border-radius: 50%;
  border: 1px solid wheat ;
  }
lable{
  font-size: 25px;
  font-weight: bold;
}
table{
  margin: 10px auto;
  font-size: 18px;
}
</style>
