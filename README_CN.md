# Knative 学习
knative 学习路径

[Knative入门——构建基于 Kubernetes 的现代化Serverless应用（servicemesher）](https://github.com/servicemesher/getting-started-with-knative)

## 第一步: Knative 是什么？ 
[官方学习手册](https://knative.dev/)


## 第二步: 准备
学习路径:  Docker -> Kubernetes -> Istio -> Knative
[Serverless CNCF 白皮书](https://github.com/cncf/wg-serverless/blob/master/whitepapers/serverless-overview/cncf_serverless_whitepaper_v1.0.pdf)

- 如果你想学习如何使用 Knative，建议直接参考第三第四步，只要知道怎么使用 Knative 部署自己的应用就可以了；
- 如果你想了解 Knative 是如何工作的，学习甚至开发维护无服务的平台，那么请继续第五六七步。

## 第三步: 试用
[Google Cloud Run](https://cloud.google.com/run/) is [GA](https://cloud.google.com/blog/products/serverless/knative-based-cloud-run-services-are-ga)ed in November 15, 2019.

[Openshift Serverless 通过 serverless operator 安装 knative](https://www.openshift.com/learn/topics/serverless)

阿里云目前在容器服务 Kubernetes 中提供了[启动 Knative 的功能](https://help.aliyun.com/document_detail/126413.html?spm=5176.11065259.1996646101.searchclickresult.378714c1qH1HBy&aly_as=VJ3VDkRt)

## 第四步：创建你的应用

基于 Knative Serverless 技术实现天气服务
  - [上篇](https://yq.aliyun.com/articles/719863)
  - [下篇](https://yq.aliyun.com/articles/720585)

[Knative 实战：一个微服务应用的部署](https://www.infoq.cn/article/gomF505vF7ONLMGllOC7)

[在Knative 上实现 Tracing 分布式追踪](https://help.aliyun.com/document_detail/122014.html)

[Official Samples](https://github.com/knative/docs/tree/master/docs/serving/samples)

[Awesome examples in cloud run](https://github.com/steren/awesome-cloudrun)

[Knative 系列（一）：基本概念和原理解读](https://www.infoq.cn/article/PEOIcPk4lZRg-fAwry8H)

[Knative 系列（二）：兵马未动粮草先行之 Build 篇](https://www.infoq.cn/article/D489mKhQ96dGwfj*w05E)

[Knative 系列（三）：Serving ](https://www.infoq.cn/article/PYGUCS*yWxhLM5Rok9vF)

[Knative 系列（四）：Eventing 篇](https://www.infoq.cn/article/FkKfwsvpVdC_60DfxMMg)

Other tutorial for knative
- https://github.com/meteatamel/knative-tutorial
- https://github.com/redhat-developer-demos/knative-tutorial

## 第五步: Knative 工作原理
https://github.com/knative

## 第六步: Tips
For instance: https://github.com/cppforlife/knctl/blob/master/docs/kubectl-plugin.md

## 第七步: 更多

Python Client https://github.com/kubernetes-client/python/blob/v10.0.1/kubernetes/docs/CustomObjectsApi.md

Knative系列列公开课（开源技术 * IBM 微讲堂）
https://developer.ibm.com/cn/os-academy-knative/
每周四晚8点档
- 09⽉月19⽇日 《Knative概览》
- 09⽉月26⽇日 《Tekton从源码构建容器器镜像》
- 10⽉月10⽇日 《Knative Serving让容器器从另扩展到⽆无限》
- 10⽉月17⽇日 《Knative Eventing打造标准云原⽣生事件平台》
- 10⽉月24⽇日 《Knative客户端⼯工具介绍》
- 10⽉月31⽇日 《案例例分享：在DevOps场景中使⽤用Knative》

