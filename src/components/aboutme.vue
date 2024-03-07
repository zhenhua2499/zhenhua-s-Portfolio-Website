<template>
    <a name="about"></a>
    <v-container>

        <section class="mt-15">
            <h4 class="text-h4 text-center mb-5">实习经历与奖项</h4>
            <v-row class="align-center justify-center">
                <v-col>

                    <v-card class="text-center pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                        <v-card-subtitle class="text-h6 text-black">实习经历</v-card-subtitle>
                        <h4 class="display-1 text-left font-weight-regular mt-5">
                            南昌市云擎科技有限公司<br>
                            Vue.js  前端开发软件部门 2024年1月至2024年2月<br><br>
                            本次实习中，我们团队致力于制作一个证书信息管理系统。在该项目中， 我的主要工作是使用Vue框架和Vuetify制作精美的前
                            端页面，用户可在前端页面中实现证书的CRUD功能。<br><br>

                            本次实习中我充分利用自身外语优势，在全英文的环境下学习Html, CSS, javascript, typescript, Vue.js,和vuetify。通过大
                            量阅读全英文官方文档学习编程语言和Vue.js框架的基础知识，浏览各大国外技术网站(比如stackoverflow, geeksforgeeks,
                            medium, Vue.js community and so on)提升码力，加入技术社区与国际码农交流心得分享经验，学习使用各种AI工具
                            （Chat-gpt, GoogleGemini, Github copilot, copilot）辅助完成了项目中前端design, coding and deployment.
                        </h4>
                        

                    </v-card>
                </v-col>
                <v-col>
                    <v-card class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                        <v-card-subtitle class="text-black text-center text-h6">荣誉奖项
                        </v-card-subtitle>
                        <div class="py-1" v-for="(item, index) in items" :key="index">
                            <label>{{ item.title }}</label>
                        
                        </div>
                    </v-card>
                </v-col>
            </v-row>
        </section>
    </v-container>
</template>

<script>
export default {
    name: "SiteAbout",
    data: () => ({

        drawer: null,
        items: [
            { title: '国家级大学生创新创业训练项目(负责人)', value: 90, color: 'cyan accent-3' },
            { title: '第八届全国大学生光电设计大赛国家三等奖', value: 100, color: 'teal' },
            { title: '全国大学生英语竞赛二等奖', value: 90, color: 'deep-orange' },
            { title: '海信杯第二届吉林省大学生人工智能创新大赛(计算机视觉方向)-等奖', value: 65, color: 'green' },
            { title: '2020吉林省高校大学生机器人竞赛(智能车方向)-等奖', value: 80, color: 'brown darken-1' },
            { title: '第八届全国大学生光电设计大赛东北赛区-等奖', value: 90, color: 'black' },
            { title: '(第三届)全国大学生嵌入式芯片与系统设计竞赛暨(第五届)智能互联创新大赛北部赛区二等奖', value: 65, color: 'red' },
            { title: '第十四届iCAN国际创新创业大赛吉林省赛区三等奖', value: 50, color: 'teal darken-2' },
        ],
    }),
}
</script>