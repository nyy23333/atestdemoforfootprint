<template>
  <el-container style="height: 100%;" class="is-vertical">
    <Header />
    <el-container>
      <Sidebar :data="menuData" />
      <el-main>
        <h3>重构布局</h3>
        <nuxt />
      </el-main>
    </el-container>
  </el-container>
</template>



<script>
import Header from './components/Header'
import Sidebar from './components/Sidebar'
import MenuData from './menu-data'
export default{
  name:'DefaultLayouts',
  components:{Header,Sidebar},
  data() {
    return {
      menuData: MenuData
    }
  }
}
</script>

<style>
html,
body,
#__nuxt,
#__layout,
#__layout {
  height: 100%;
  margin: 0;
  padding: 0;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
