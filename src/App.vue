<script>
import Vue from 'vue';
import { Layout, Header, Content, Footer, Menu, MenuItem, Icon, Card, Breadcrumb, BreadcrumbItem, Sider, Submenu } from 'iview';
Vue.component('Layout', Layout);
Vue.component('Header', Header);
Vue.component('Content', Content);
Vue.component('Footer', Footer);
Vue.component('Menu', Menu);
Vue.component('MenuItem', MenuItem);
Vue.component('Icon', Icon);
Vue.component('Card', Card);
Vue.component('Breadcrumb', Breadcrumb);
Vue.component('BreadcrumbItem', BreadcrumbItem);
Vue.component('Sider', Sider);
Vue.component('Submenu', Submenu);

export default {
  data(){
    return{

    }
  }
}

</script>
<style scoped>
.layout {
  background: #fff;
  position: relative;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
.mainBox {
  position: absolute;
  min-height: 100%;
  width: 100%;
}
.main {
  flex: 1;
  position: relative;
}

.layout-logo {
  width: 100px;
  height: 30px;
  background: #fff;
  border-radius: 3px;
  float: left;
  position: relative;
  top: 15px;
  left: 20px;
}

.layout-nav {
  width: 420px;
  margin: 0 auto;
  margin-right: 20px;
}

.layout-footer-center {
  text-align: center;
}

</style>
<template>
  <div class="layout">
    <Header>
      <Menu mode="horizontal" theme="dark" active-name="1">
        <div class="layout-logo"></div>
        <div class="layout-nav">
          <MenuItem name="1">
          <Icon type="ios-navigate"></Icon>
          网站首页
          </MenuItem>
          <MenuItem name="2">
          <Icon type="ios-keypad"></Icon>
          退出登陆
          </MenuItem>
        </div>
      </Menu>
    </Header>
    <Layout class="main">
      <Content :style="{padding: '0 0',minHeight:'100%',width:'100%',position:'absolute'}">
        <Layout class="mainBox">
          <Sider hide-trigger :style="{background: '#fff'}">
            <Menu active-name="1-2" theme="light" width="auto" :open-names="['1']">
              <Submenu name="1">
                <template slot="title">
                  <Icon type="gear-b"></Icon>
                  商品管理
                </template>
                <MenuItem name="1-1">商品分类</MenuItem>
                <MenuItem name="1-2">品牌管理</MenuItem>
                <MenuItem name="1-3">商品列表</MenuItem>
                <MenuItem name="1-4">商品审核</MenuItem>
                <MenuItem name="1-5">商品评价</MenuItem>
              </Submenu>
              <Submenu name="2">
                <template slot="title">
                  <Icon type="navicon-round"></Icon>
                  订单管理
                </template>
                <MenuItem name="2-1">订单列表</MenuItem>
                <MenuItem name="2-2">订单投诉</MenuItem>
                <MenuItem name="2-3">退款列表</MenuItem>
                <MenuItem name="2-4">订单结算</MenuItem>
              </Submenu>
              <Submenu name="3">
                <template slot="title">
                  <Icon type="document"></Icon>
                  报表统计
                </template>
                <MenuItem name="3-1">销售订单统计</MenuItem>
                <MenuItem name="3-2">商品销售统计</MenuItem>
                <MenuItem name="3-3">店铺销售统计</MenuItem>
                <MenuItem name="3-4">销售额统计</MenuItem>
                <MenuItem name="3-5">新增会员统计</MenuItem>
                <MenuItem name="3-6">会员登录统计</MenuItem>
              </Submenu>
              <Submenu name="4">
                <template slot="title">
                  <Icon type="ios-crop-strong"></Icon>
                  资金管理
                </template>
                <MenuItem name="3-1">提现管理</MenuItem>
                <MenuItem name="3-2">资金流水</MenuItem>
              </Submenu>
              <Submenu name="5">
                <template slot="title">
                  <Icon type="link"></Icon>
                  店铺管理
                </template>
                <MenuItem name="3-1">添加店铺</MenuItem>
                <MenuItem name="3-2">店铺列表</MenuItem>
                <MenuItem name="3-2">店铺审核</MenuItem>
              </Submenu>
              <Submenu name="6">
                <template slot="title">
                  <Icon type="link"></Icon>
                  会员管理
                </template>
                <MenuItem name="3-1">会员等级</MenuItem>
                <MenuItem name="3-2">会员列表</MenuItem>
                <MenuItem name="3-2">添加会员</MenuItem>
                <MenuItem name="3-2">账号管理</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  分销管理
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  促销管理
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  地区管理
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  文章管理
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  系统管理
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
              <Submenu name="7">
                <template slot="title">
                  <Icon type="link"></Icon>
                  商城设置
                </template>
                <MenuItem name="7-1">分销商家列表</MenuItem>
                <MenuItem name="7-1">分销商品列表</MenuItem>
                <MenuItem name="7-1">佣金分成列表</MenuItem>
                <MenuItem name="7-1">推广用户列表</MenuItem>
              </Submenu>
            </Menu>
          </Sider>
          <Layout :style="{padding: '0 24px 24px'}">
            <Breadcrumb :style="{margin: '24px 0'}">
              <BreadcrumbItem>Home</BreadcrumbItem>
              <BreadcrumbItem>Components</BreadcrumbItem>
              <BreadcrumbItem>Layout</BreadcrumbItem>
            </Breadcrumb>
            <Content :style="{padding: '24px', minHeight: '280px', background: '#fff'}">
              <router-view></router-view>
            </Content>
            <Footer class="layout-footer-center">2011-2016 &copy; iallenaugustine@gmail.com</Footer>
          </Layout>
        </Layout>
      </Content>
    </Layout>
  </div>
</template>
