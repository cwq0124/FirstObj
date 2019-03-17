<!--  -->
<template>
  <div>
    <div class="layout">
        <Layout>
            <Header>
                <Menu mode="horizontal" theme="dark" active-name="1">
                    <div class="layout-nav">
                        <MenuItem name="1">
                            <Icon type="ios-navigate"></Icon>
                            Item 1
                        </MenuItem>
                        <MenuItem name="2">
                            <Icon type="ios-keypad"></Icon>
                            Item 2
                        </MenuItem>
                        <MenuItem name="3">
                            <Icon type="ios-analytics"></Icon>
                            Item 3
                        </MenuItem>
                        <MenuItem name="4">
                            <Icon type="ios-paper"></Icon>
                            Item 4
                        </MenuItem>
                    </div>
                </Menu>
            </Header>
            <Content :style="{padding: '0 50px'}">
                <Breadcrumb :style="{margin: '20px 0'}">
                    <BreadcrumbItem>Home</BreadcrumbItem>
                    <BreadcrumbItem>Components</BreadcrumbItem>
                    <BreadcrumbItem>Layout</BreadcrumbItem>
                </Breadcrumb>
                <Card>
                    <div style="min-height: 400px;">
                         <!-- <Card style="width:320px" class="inner-card">
                            <div style="text-align:center">
                                <img src="../assets/logo.png">
                                <h3>A high quality UI Toolkit based on Vue.js</h3>
                            </div>
                        </Card> -->
                        <!-- <Collapse v-model="value2" accordion class="coll">
                            <Panel name="1">
                                史蒂夫·乔布斯
                                <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                            </Panel>
                            <Panel name="2">
                                斯蒂夫·盖瑞·沃兹尼亚克
                                <p slot="content">斯蒂夫·盖瑞·沃兹尼亚克（Stephen Gary Wozniak），美国电脑工程师，曾与史蒂夫·乔布斯合伙创立苹果电脑（今之苹果公司）。斯蒂夫·盖瑞·沃兹尼亚克曾就读于美国科罗拉多大学，后转学入美国著名高等学府加州大学伯克利分校（UC Berkeley）并获得电机工程及计算机（EECS）本科学位（1987年）。</p>
                            </Panel>
                            <Panel name="3">
                                乔纳森·伊夫
                                <p slot="content">乔纳森·伊夫是一位工业设计师，现任Apple公司设计师兼资深副总裁，英国爵士。他曾参与设计了iPod，iMac，iPhone，iPad等众多苹果产品。除了乔布斯，他是对苹果那些著名的产品最有影响力的人。</p>
                            </Panel>
                        </Collapse> -->
                        <!--侧面菜单-->
                            <Row>
                                <Col span="8">
                                    <Menu :theme="theme2">
                                        <Submenu name="1">
                                            <template slot="title">
                                                <Icon type="ios-paper" />
                                                内容管理
                                            </template>
                                            <MenuItem name="1-1">文章管理</MenuItem>
                                            <MenuItem name="1-2">评论管理</MenuItem>
                                            <MenuItem name="1-3">举报管理</MenuItem>
                                        </Submenu>
                                        <Submenu name="2">
                                            <template slot="title">
                                                <Icon type="ios-people" />
                                                用户管理
                                            </template>
                                            <MenuItem name="2-1">新增用户</MenuItem>
                                            <MenuItem name="2-2">活跃用户</MenuItem>
                                        </Submenu>
                                        <Submenu name="3">
                                            <template slot="title">
                                                <Icon type="ios-stats" />
                                                统计分析
                                            </template>
                                            <MenuGroup title="使用">
                                                <MenuItem name="3-1">新增和启动</MenuItem>
                                                <MenuItem name="3-2">活跃分析</MenuItem>
                                                <MenuItem name="3-3">时段分析</MenuItem>
                                            </MenuGroup>
                                            <MenuGroup title="留存">
                                                <MenuItem name="3-4">用户留存</MenuItem>
                                                <MenuItem name="3-5">流失用户</MenuItem>
                                            </MenuGroup>
                                        </Submenu>
                                    </Menu>
                                </Col>
                                </Row>
                    </div>
                    <Button shape="circle" type="primary" title="这是一个测试">test</Button>
                </Card>
            </Content>
            <Footer class="layout-footer-center">2011-2016 &copy; TalkingData</Footer>
        </Layout>
        </div>
    <!-- <Button type="primary" shape="circle" icon="ios-search" size="large" @click="test">测试</Button> -->
    <!-- <Button type="primary" @click="modal1 = true">Display dialog box</Button>
    <Modal
        v-model="modal1"
        title="Common Modal dialog box title"
        @on-ok="ok"
        @on-cancel="cancel">
        <p>Content of dialog</p>
        <p>Content of dialog</p>
        <p>Content of dialog</p>
    </Modal>
    <DatePicker type="date" confirm placeholder="Select date" style="width: 200px"></DatePicker>
    <p class="style1">test</p>
    <BackTop :height="100" :bottom="50"></BackTop> -->
     <!-- <Card style="width:350px;float:right">
        <p slot="title">
            <Icon type="ios-film-outline"></Icon>
            Classic film
        </p>
        <a href="#" slot="extra" @click.prevent="changeLimit">
            <Icon type="ios-loop-strong"></Icon>
            Change
        </a>
        <ul>
            <li v-for="(item,index) in movieList" :key="index">
                <a :href="item.url" target="_blank" class="item">{{ item.name }}</a>
                <span>
                  <Rate allow-half v-model="item.rate" disabled show-text>{{ item.rate }}</Rate>
                </span>
            </li>
        </ul>
    </Card> -->
  </div>
</template>
<script>
export default {
  data () {
    return {
      value2: '1'
    }
  },

  components: {},

  computed: {},

  methods: {
  }
}
</script>
<style>
.style1{
  margin:20px;
  height:600px;
  background-color: #5cadff;
}
/* .content{
  position:relative;
} */
.inner-card{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
}
.layout-logo{
    width: 100px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 15px;
    left: 20px;
}
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}
.layout-footer-center{
    text-align: center;
}
.coll{
    width:400px;
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>
