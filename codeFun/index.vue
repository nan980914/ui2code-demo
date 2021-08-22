<template>
  <div class="flex-col container">
    <div class="flex-col header">
      <div class="justify-center group">
        <div class="flex-row group_1">
          <img
            src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460495736697.png"
            class="image"
          />
          <img
            src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460472402413.png"
            class="image_1"
          />
        </div>
        <span class="text">9:53 AM</span>
        <div class="flex-row group_2">
          <img
            src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460446684045.png"
            class="image_2"
          />
          <span class="text_1">100%</span>
          <img
            src="https://project-user-resource-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16292159862934909493.png"
            class="image_3"
          />
        </div>
      </div>
      <div class="justify-center group_3">
        <span>订单中心</span>
        <div class="flex-row section_1">
          <div class="left-image-wrapper flex-col items-center view">
            <img
              src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460406269510.png"
              class="image_4"
            />
          </div>
          <div class="section_2"></div>
          <div class="left-image-wrapper flex-col items-center view_1">
            <img
              src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460364921877.png"
              class="image_5"
            />
          </div>
        </div>
      </div>
    </div>
    <div class="flex-col group_4">
      <div class="flex-col section_3">
        <div class="flex-row section_4">
          <img
            src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674472947416676.png"
            class="image_6"
          />
          <span class="text_3">您有1个新的待处理订单，为空调清洗服务项…</span>
          <img
            src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674473232232618.png"
            class="image_7"
          />
        </div>
        <div class="flex-col group_5">
          <div class="flex-col group_6">
            <div class="justify-center group_7">
              <span>今日收入（元）</span>
              <img
                src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674472334859877.png"
                class="image_8"
              />
            </div>
            <span class="text_5">12.00</span>
          </div>
          <div class="flex-col group_8">
            <div class="divider"></div>
            <div class="flex-row equal-division">
              <div class="equal-division-item flex-col items-center group_9">
                <span class="text_6">待收入（元）</span>
                <span class="text_7 text_8">12.00</span>
              </div>
              <div class="horiz-divider"></div>
              <div class="equal-division-item flex-col items-center group_10">
                <span class="text_9">累计收入（元）</span>
                <span class="text_7 text_10">128.00</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="flex-col group_11">
        <div class="flex-col group_12">
          <div class="flex-col section_5">
            <div class="justify-between group_13">
              <div class="flex-row group_14">
                <img
                  src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674468244119509.png"
                  class="image_9"
                />
                <span class="text_11">订单管理</span>
              </div>
              <div class="flex-row group_15">
                <span>全部订单</span>
                <img
                  src="https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674460512982194.png"
                  class="image_10"
                />
              </div>
            </div>
            <div class="divider_1"></div>
            <div class="flex-row equal-division_1">
              <div class="equal-division-item flex-col items-center group_16">
                <span class="text_13">待确认订单</span>
                <span class="text_7 text_14">1</span>
              </div>
              <div class="horiz-divider_1"></div>
              <div class="equal-division-item flex-col items-center group_17">
                <span class="text_15">待处理订单</span>
                <span class="text_7 text_16">0</span>
              </div>
              <div class="horiz-divider_1"></div>
              <div class="equal-division-item flex-col items-center group_18">
                <span class="text_17">售后订单</span>
                <span class="text_7 text_18">1</span>
              </div>
            </div>
          </div>
          <div class="flex-col list">
            <template v-for="(item, i) in orderList">
              <div class="list-item flex-col" :key="'item' + i">
                <div class="group_19 justify-between">
                  <div class="left-group flex-row">
                    <span>{{ item.timeTitile }}</span>
                    <span>{{ item.time }}</span>
                    <span class="text_21">{{ item.day }}</span>
                  </div>
                  <span class="text_23">{{ item.status }}</span>
                </div>
                <div class="group_20 justify-between">
                  <div class="flex-row">
                    <span class="text_25">{{ item.name }}</span>
                    <span class="text_27">{{ item.phone }}</span>
                    <img class="image_11" :src="item.phoneImg" />
                  </div>
                  <div class="right-text-wrapper flex-col items-center">
                    <span>{{ item.type }}</span>
                  </div>
                </div>
                <div class="section_9 justify-between">
                  <div class="flex-row">
                    <img class="image_13" :src="item.orderImg" />
                    <div class="right-group flex-col">
                      <div class="top-group flex-col">
                        <span class="text_30">{{ item.orderName }}</span>
                        <span class="text_32">{{ item.orderInfo }}</span>
                      </div>
                      <span class="text_34">{{ item.money }}</span>
                    </div>
                  </div>
                  <span class="text_36">{{ item.number }}</span>
                </div>
                <div class="group_23">
                  <span class="text_38">{{ item.total }}</span>
                  <span class="text_40">{{ item.actural }}</span>
                </div>
                <div class="group_24 justify-end">
                  <div class="left-text-wrapper flex-col items-center">
                    <span>{{ item.cancel }}</span>
                  </div>
                  <div class="right-text-wrapper_1 flex-col items-center">
                    <span>{{ item.confirm }}</span>
                  </div>
                </div>
              </div>
            </template>
          </div>
        </div>
        <div class="justify-center button">
          <div class="left-section"></div>
          <span class="text_78">暂无更多信息</span>
          <div class="left-section view_38"></div>
        </div>
      </div>
    </div>
    <div class="justify-between tab-bar">
      <div class="left-group_1 flex-col items-center view_39">
        <img
          src="https://project-user-resource-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16292159865861550020.png"
          class="image_19"
        />
        <span>首页</span>
      </div>
      <div class="left-group_1 flex-col items-center view_40">
        <img
          src="https://project-user-resource-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16292159865873492905.png"
          class="image_19"
        />
        <span>订单</span>
      </div>
      <div class="left-group_1 flex-col items-center view_41">
        <img
          src="https://project-user-resource-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16292159865876616041.png"
          class="image_19"
        />
        <span>我的</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      orderList: [
        {
          timeTitile: "服务时间：",
          time: "2020/08/12",
          day: "上午",
          status: "服务中",
          name: "刘美丽",
          phone: "15032547844",
          phoneImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674471376503557.png",
          type: "粉丝单",
          orderImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674469281769685.png",
          orderName: "洗衣机深度清洗",
          orderInfo: "滚桶洗衣机全拆洗(带烘干)",
          money: "¥199.00/台",
          number: "x3",
          total: "总计￥597.00，",
          actural: "实付¥497.00",
          cancel: "取消订单",
          confirm: "完成服务",
        },
        {
          timeTitile: "服务时间：",
          time: "2020/08/12",
          day: "13:00-13:30",
          status: "售后中",
          name: "刘美丽",
          phone: "15032547844",
          phoneImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674471376503557.png",
          type: "公海单",
          orderImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674469281769685.png",
          orderName: "洗衣机深度清洗",
          orderInfo: "滚桶洗衣机全拆洗(带烘干)",
          money: "¥199.00/台",
          number: "x3",
          total: "售后订单",
          actural: null,
          cancel: "取消订单",
          confirm: "完成售后",
        },
        {
          timeTitile: "服务时间：",
          time: "2020/08/12",
          day: "13:00-13:30",
          status: "售后中",
          name: "刘美丽",
          phone: "15032547844",
          phoneImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674471376503557.png",
          type: "公海单",
          orderImg:
            "https://codefun-proj-user-res-1256085488.cos.ap-guangzhou.myqcloud.com/611924cd6b68fa00119f30a0/611a11c16b68fa00119f4e9f/16293674469281769685.png",
          orderName: "洗衣机深度清洗",
          orderInfo: "滚桶洗衣机全拆洗(带烘干)",
          money: "¥199.00/台",
          number: "x3",
          total: "售后订单",
          actural: null,
          cancel: "取消订单",
          confirm: "完成售后",
        },
      ],
    };
  },
};
</script>

<style src="./index.css" />