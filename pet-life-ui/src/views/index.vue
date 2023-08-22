<template>
  <div class="app-container home">
    <el-row :gutter="20">
      <el-col :span="6">
        <img
          src="../assets/logo/logo.png"
          alt=""
          width="150px"
          style="margin-left: 20%"
        />
      </el-col>
      <el-col :sm="24" :lg="12" style="padding-left: 20px" :span="12">
        <h2>宠物贴贴后台管理系统</h2>
        <p>
          宠物贴贴后台管理系统是一款针对“宠物贴贴微信小程序”所设计的管理系统，旨在帮助宠物贴贴的管理员高效地管理和维护“宠物贴贴小程序”的各项业务。该后台管理系统提供了丰富的管理功能，包括用户管理、内容管理、社区管理等多种功能。管理员可以通过该系统轻松地对宠物贴贴小程序进行管理和运营。
        </p>
      </el-col>
    </el-row>
    <el-divider />
    <el-row :gutter="20">
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>用户管理主要包括以下几个模块</span>
          </div>
          <div class="body">
            <ul style="margin-top: 10px">
              <li>用户管理：对小程序用户信息进行删改查</li>
              <el-divider></el-divider>
              <li>积分管理：对用户的签到积分进行删改查</li>
              <el-divider></el-divider>
              <li>宠物管理：对用户发布的宠物信息进行删改查</li>
              <el-divider></el-divider>
              <li>寻宠管理：对用户发布的寻宠信息进行删改查</li>
            </ul>
          </div>
        </el-card>
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>内容管理主要包括以下几个模块</span>
          </div>
          <div class="body">
            <ul style="margin-top: 10px">
              <li>答题管理：主要用于新增每日一题</li>
              <el-divider></el-divider>
              <li>文章管理：主要用于新增首页文章</li>
              <el-divider></el-divider>
              <li>科普管理：主要用于新增宠物科普</li>
            </ul>
          </div>
        </el-card>
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>社区管理主要包括以下几个模块</span>
          </div>
          <div class="body">
            <ul style="margin-top: 10px">
              <li>动态管理：对用户发表的动态进行删改查</li>
              <el-divider></el-divider>
              <li>聊天管理：对用户的聊天记录进行删改查</li>
              <el-divider></el-divider>
              <li>评论管理：对用户的评论信息进行删改查</li>
            </ul>
          </div>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "Index",
  data() {
    return {
      // 版本号
      version: "3.8.1",
    };
  },
  methods: {
    goTarget(href) {
      window.open(href, "_blank");
    },
  },
};
</script>

<style scoped lang="scss">
.home {
  blockquote {
    padding: 10px 20px;
    margin: 0 0 20px;
    font-size: 17.5px;
    border-left: 5px solid #eee;
  }
  hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid #eee;
  }
  .col-item {
    margin-bottom: 20px;
  }

  ul {
    padding: 0;
    margin: 0;
  }

  font-family: "open sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  color: #676a6c;
  overflow-x: hidden;

  ul {
    list-style-type: none;
  }

  h4 {
    margin-top: 0px;
  }

  h2 {
    margin-top: 10px;
    font-size: 26px;
    font-weight: 100;
  }

  p {
    margin-top: 10px;

    b {
      font-weight: 700;
    }
  }

  .update-log {
    ol {
      display: block;
      list-style-type: decimal;
      margin-block-start: 1em;
      margin-block-end: 1em;
      margin-inline-start: 0;
      margin-inline-end: 0;
      padding-inline-start: 40px;
    }
  }
}
</style>

