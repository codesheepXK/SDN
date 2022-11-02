<template>
    <el-menu
        text-color="#fff"
        default-active="1"
        class="menu"
    >
        <el-menu-item index="1" >
        <span>首页</span>
        </el-menu-item>
        <el-sub-menu index="2" class="sub-menu">
            <template #title>
                <span >流量监控中心</span>
            </template>
        <el-menu-item index="2-1" >全局流量监控</el-menu-item>
        <el-menu-item index="2-2" >端口流向流量监控</el-menu-item>
        <el-menu-item index="2-3" >可选度量值监控</el-menu-item>
        </el-sub-menu>

        <el-sub-menu index="3" class="sub-menu">
            <template #title>
                <span >设备信息</span>
            </template>
        <el-menu-item index="3-1" >交换机信息</el-menu-item>
        <el-menu-item index="3-2" >主机信息</el-menu-item>
        <el-menu-item index="3-3" >数据信息</el-menu-item>
        <el-menu-item index="3-4" >设备信息查询</el-menu-item>
        </el-sub-menu>

        <el-sub-menu index="4" class="sub-menu">
            <template #title>
                <span >流表管理</span>
            </template>
        <el-menu-item index="4-1" >下发流表</el-menu-item>
        <el-menu-item index="4-2" >流表信息</el-menu-item>
        </el-sub-menu>

        <el-sub-menu index="5" class="sub-menu">
            <template #title>
                <span >安全防护</span>
            </template>
        <el-menu-item index="5-1" >安全检测</el-menu-item>
        <el-menu-item index="5-2" >主动防御</el-menu-item>
        </el-sub-menu>

        <el-menu-item index="6" >
        <span>智能流量调度</span>
        </el-menu-item>
        <el-menu-item index="7" >
        <span>日志管理</span>
        </el-menu-item>
        <el-menu-item index="8" >
        <span>权限管理</span>
        </el-menu-item>

    </el-menu>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.menu{
    width: 15%;
    min-width: 200px;
    height: 90vh;
    background-color: rgb(48,48,75);
    color: #fff;
    border: 0px;
    overflow: auto;
    &::-webkit-scrollbar{
         display:none
    }
}
.el-sub-menu{
    .el-menu-item{
        background-color: rgb(18,25,39);
        &:hover{
            color:  rgb(67, 197, 240) ;
        }
    }
}
.el-menu-item.is-active{
    color: #fff !important;
    background-color: rgb(24, 166, 213) !important;
}
.menu>.el-menu-item:hover {
    color:  rgb(67, 197, 240);
    background-color: rgb(48,48,75) ;
}
::v-deep .el-sub-menu__title:hover{
    span{
        color: rgb(67, 197, 240) !important;
    }
   background-color: rgb(48,48,75) !important;
}
::v-deep.is-opened .el-sub-menu__title{
    color:  rgb(67, 197, 240) !important; 
}
</style>