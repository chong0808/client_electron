<template>
  <div class="listbox">
		<el-row class="el-memu-box">
      <el-col :span="24">
        <el-menu default-active="/subject/todayManage"  class="el-memu-list" :router='true'> 
          <el-menu-item index="/subject/todayManage">
            <i class="el-icon-menu"></i>
            <span slot="title">今日课表</span>
          </el-menu-item>
          <el-menu-item index="/subject/teacherManage">
            <i class="el-icon-menu"></i>
            <span slot="title">老师课表</span>
          </el-menu-item>
          <el-menu-item index="/subject/subjectManage">
            <i class="el-icon-setting"></i>
            <span slot="title">课程管理</span>
          </el-menu-item>
          <el-menu-item index="/subject/awaitDo">
            <i class="el-icon-setting"></i>
            <span slot="title">待排课</span>
          </el-menu-item>
          <el-menu-item index="/subject/awaitManage">
            <i class="el-icon-setting"></i>
            <span slot="title">待处理</span>
          </el-menu-item>
        </el-menu>
      </el-col>
    </el-row>
	</div>
</template>
<script>
    export default {
        data () {
          return {
                title: 'statistical',
                isCollapse: true
          }
        }
    }
</script>
<style scoped>

.listbox{
    height: 100%;
    position: absolute;
    left: 50px;
    background: #FFF;
    padding-bottom: 52px;
    padding-top: 45px;
    top: 0;
	  width: 200px;
}
.el-memu-box,
.el-memu-box>div{
  height: 100%;
}
.el-memu-list{
  height: 100%;
}
</style>