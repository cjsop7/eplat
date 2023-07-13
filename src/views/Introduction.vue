<template>
    <v-container>
        <v-card>
            <v-card-title class="text-h4 ml-2 mt-2">회사 소개<v-spacer/>English Platform<v-spacer/></v-card-title>
            <v-card-text>
                <v-container class="pa-2" elevation="0">
                    <v-row v-for="item in items" :key="item.title">
                        <v-col cols="2">
                            <v-container class="fill-height">
                                <v-img :src=item.image />
                            </v-container>
                        </v-col>
                        <v-col cols="10" class="pl-5">
                            <br>
                            <span class="text-h6">{{item.title}}</span><br>
                            <span class="text-body-2">{{ item.content }}</span>
                        </v-col>
                    </v-row>
                    
                </v-container>
            </v-card-text>
        </v-card>
        <v-card class="mt-5">
            <v-card-title class="text-h4 ml-2 mt-2">연혁<v-spacer/>English Platform<v-spacer/></v-card-title>
            <v-card-text class="text-body-1">
                2023 - 이플렛 영어교재출판 (60종)<br>
                2020 - 이플렛 영어교재 및 교구개발<br>
                2019 - 로그아이1.0 영어교재출판 <br>
                2006 - 이지잉글리쉬 영어교재 출판<br>
                2005 - 이지 화상영어센타 외국현지 법인설립<br>
                2002 - 이지아이외국어학원 설립<br>
                2001 - 이지아이입시학원 설립<br>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<script setup lang="ts">
import firstImage from '@/assets/intro_1.jpg'
import secondImage from '@/assets/intro_2.jpg'
import thirdImage from '@/assets/intro_3.jpg'
import fourthImage from '@/assets/intro_4.jpg'

const items = [
    {title: '교재개발', content: 'E-plat 은 오랜 기간 현장에서의 지도경험을 통해 창의적이고 융합적인 놀이식 학습방법을 개발하여 보급하고 있습니다. 또한 국내외 여러 나라와 지역에서 다양한 현장경험이 있는 선생님들의 차별화 된 교육방법을 제품화 하여 함께 비전을 공유할 수 있는 공간을 제공하고 있습니다.', image:firstImage},
    {title: '교구개발', content: '영어를 처음 시작하는 아이들에게는 결과에 중점을 두는 것이 아니라 아이들이 좋아하는 놀이중심으로 과정에 충실해야한다고 생각합니다. 따라서 E-plat 은 교재와 함께 활용할 수 있는 다양한 교구도 함께 개발하고 있습니다.', image:secondImage},
    {title: '온라인개발', content: 'E-plat 의 온라인 개발팀은 원어민과 프로그램전공자 그리고 오랜 기간 외국어학원의 운영경험을 기반으로 여러 영어교육회사의 학습시스템을 개발하여 제공하고 있습니다.', image:thirdImage},
    {title: '교육개발 및 강사교육', content: 'E-plat 의 교육은 유치부 교육과 초등부 교육으로 이원화 되어 있으며 다양한 놀이식 학습시스템과 교구의 활용방법을 보급하고 있습니다.', image:fourthImage},
]
</script>

<style scoped></style>