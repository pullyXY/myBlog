<template>
  <div class="artical_all">
    <a-card class="card" title="这里是标题" :hoverable="true">
      <a href="#" slot="extra">more</a>
      <p class="outline">这里是内容概要</p>
      <p>
        这里是内容
        <br>...
      </p>
      <a-divider dashed/>
      <a-icon class="tips" type="message"/>
      <span class="tips tipss">0</span>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="tag"/>
      <a-tag class="tips tipss" color="pink">pink</a-tag>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="folder"/>
      <a-tag class="tips tipss" color="purple">purple</a-tag>
    </a-card>
    <a-card class="card" title="这里是标题" :hoverable="true">
      <a href="#" slot="extra">more</a>
      <p class="outline">这里是内容概要</p>
      <p>
        这里是内容
        <br>...
      </p>
      <a-divider dashed/>
      <a-icon class="tips" type="message"/>
      <span class="tips tipss">0</span>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="tag"/>
      <a-tag class="tips tipss" color="pink">pink</a-tag>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="folder"/>
      <a-tag class="tips tipss" color="purple">purple</a-tag>
    </a-card>
    <a-card class="card" title="这里是标题" :hoverable="true">
      <a href="#" slot="extra">more</a>
      <p class="outline">这里是内容概要</p>
      <p>
        这里是内容
        <br>...
      </p>
      <a-divider dashed/>
      <a-icon class="tips" type="message"/>
      <span class="tips tipss">0</span>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="tag"/>
      <a-tag class="tips tipss" color="pink">pink</a-tag>
      <a-divider type="vertical"/>
      <a-icon class="tips" type="folder"/>
      <a-tag class="tips tipss" color="purple">purple</a-tag>
    </a-card>
    <div class="dir">
      <a-anchor >
        <a-anchor-link href="#components-anchor-demo-basic" title="Basic demo"/>
        <a-anchor-link href="#components-anchor-demo-static-anchor" title="Fixed demo"/>
        <a-anchor-link href="#API" title="API">
          <a-anchor-link href="#Anchor-Props" title="Anchor Props"/>
          <a-anchor-link href="#Link-Props" title="Link Props"/>
        </a-anchor-link>
        <a-anchor-link href="#components-anchor-demo-basic" title="Basic demo"/>
        <a-anchor-link href="#components-anchor-demo-static-anchor" title="Fixed demo"/>
        <a-anchor-link href="#components-anchor-demo-basic" title="Basic demo"/>
        <a-anchor-link href="#components-anchor-demo-static-anchor" title="Fixed demo"/>
      </a-anchor>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {}
};
</script>

<style>
.card {
  text-align: left;
  margin-bottom: 10px !important;
}
.outline {
  font-size: 14px;
  font-weight: bold;
}
.tips {
  display: inline-block;
  /* margin-right:2px; */
}
.tipss {
  margin-left: 5px !important;
}
.artical_all {
  /* position: relative; */
  margin-left: 10px;
  padding-right:300px;
}
.dir {
  top: 115px;
  right: 0;

  width: 290px;
  position: fixed;
  background: #ccc;
  text-align: left;
}
</style>
