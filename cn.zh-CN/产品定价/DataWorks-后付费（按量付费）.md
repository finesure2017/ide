# DataWorks-后付费（按量付费） {#concept_264774 .concept}

开通DataWorks按量付费的方式后，即可在DataWorks进行任务开发、定时任务调度、数据同步任务调度、大规模工作流监控、数据质量监控、数据服务API调用和AppStudio开发环境代码调试等操作。

**说明：** 

-   新用户必须开通DataWorks-后付费（按量付费），旨在让您以最低的成本使用DataWorks所有基本的核心功能，享受一站式数据研发全流程。
-   DataWorks现处于公测免费阶段，欢迎您进行试用并提出宝贵的意见。当前计费价格仅供参考，具体的收费时间将另行通知。

## 计费项一览表 {#section_1ww_j0o_r27 .section}

DataWorks以按量付费的方式开通如下计费项：

-   公共调度资源组
-   公共数据集成资源组
-   智能监控基线数量
-   数据质量规则实例
-   数据服务调用次数和实际调用时间
-   AppStudio开发环境

**说明：** 

-   您使用上述相应的资源后才会进行计费。
-   开通上述计费项后，将同时为您免费开通DataWorks基础版。

详情请参见[DataWorks按量付费一览表](cn.zh-CN/产品定价/附录/DataWorks按量付费一览表.md#)。

## 公共调度资源组 {#section_58d_999_h12 .section}

-   计费范围

    所有被提交至调度系统的节点所产生的各类型实例（虚拟节点产生的实例除外），均会纳入计费范围，包括周期实例、手动实例、测试实例和补数据实例。

-   计费标准

    该计费项以6档阶梯价的形式，按日收取您每日运行实例数量所在阶梯的价格，计费标准如下表所示。

    |地域（Region）|起始实例数|结束实例数|计费周期|费用（元/日）|
    |----------|-----|-----|----|-------|
    |华东1（杭州） 华东2（上海）

 华北2（北京）

 华南 1（深圳）

 香港

 |1|10|日|0|
    |11|500|日|0.99|
    |501|5000|日|60.00|
    |5001|20000|日|150.00|
    |20001|50000|日|270.00|
    |50001|120000|日|600.00|
    |亚太东南 1（新加坡） 亚太东南 2（悉尼）

 亚太东南 3（吉隆）

 亚太东南 5（雅加达）

 亚太东北 1（东京）

 美国西部 1（硅谷）

 美国东部 1（弗吉尼亚）

 欧洲中部 1（法兰克福）

 英国（伦敦）

 中东东部 1（迪拜）

 |1|10|日|0|
    |11|500|日|1.49|
    |501|5000|日|90.00|
    |5001|20000|日|225.00|
    |20001|50000|日|405.00|
    |50001|120000|日|900.00|

    **说明：** 每日实例数量如果达到120000以上，则超出实例无法正常调度运行。如果您的实际业务量超过该上限阈值，请提交工单联系阿里云技术支持。

-   扣费方式

    计费系统在每天00:00开始，清算前一个自然日内运行成功的实例数量，并根据上述收费标准中的价格区间进行扣费，每次仅扣除一个区间的日费用，不会叠加扣费。

    例如某用户的DataWorks工作空间部署在华东2（上海）Region，在2019年4月30日共运行成功了502个实例，则在2019年5月1日00:00后，将会扣除一笔60元的费用。

-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用。此时如果您没有购买公共资源调度组资源包，则未开始运行的实例无法启动，已开始运行的实例仍可维持运行至结束。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。

## 公共数据集成资源组 {#section_6c6_037_383 .section}

-   计费范围

    数据集成任务在周期实例、补数据实例、手动实例、数据开发（DataStudio）界面业务流程、冒烟测试等几种运行方式所产生的并发，均会纳入计费范围。

    **说明：** 数据集成任务实例不仅会消耗公共数据集成资源组（按量付费），也会同时消耗公共调度资源组（按量付费）。

-   计费标准

    该计费项以6档阶梯价的形式，按日收取您每日运行数据集成任务并发数量所在阶梯的价格，计费标准如下表所示。

    |地域|起始实例数|结束实例数|计费周期|费用（元/日）|
    |--|-----|-----|----|-------|
    |华东1（杭州）|1|10|日|0|
    |华东2（上海）|11|500|日|0.99|
    |华北2（北京）|501|5000|日|6.00|
    |华南1（深圳）|5001|20000|日|20.00|
    |香港|20001|50000|日|50.00|
    | |50001|120000|日|100.00|
    |亚太东南1（新加坡） 亚太东南2（悉尼）

 亚太东南3（吉隆）

 亚太东南5（雅加达）

 亚太东北1（东京）

 美国西部1（硅谷）

 美国东部1（弗吉尼亚）

 欧洲中部1（法兰克福）

 英国（伦敦）

 中东东部1（迪拜）

 |1|10|日|0|
    |11|500|日|1.49|
    |501|5000|日|9.00|
    |5001|20000|日|30.00|
    |20001|50000|日|75.00|
    |50001|120000|日|150.00|

    **说明：** 每日实例数量如果达到120000以上，则超出实例无法正常调度运行。如果您的实际业务量超过该上限阈值，请提交工单联系阿里云技术支持。

-   扣费方式

    计费系统在每天00:00，清算前一个自然日内运行成功的实例数量，并根据上述收费标准中的价格区间进行扣费，每次仅扣除一个区间的日费用，不会叠加扣费。

    例如某用户在华东2（上海）Region的DataWorks工作空间下，配置两个同步任务A和B，使用公共资源运行任务。任务A的并发数配置为2，按天调度，每天产生1个实例。任务B的并发数配置为5，按小时调度，每天产生24个实例。

    如果所有的任务实例均运行成功，则每天收费的计算逻辑如下所示。

    1.  清算任务日累计并发数为2\*1+5\*24=122。
    2.  日并发数122处于11~500区间，查看该区间的价格，即扣除单日费用0.99元。
-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用。此时如果您没有购买公共资源调度组资源包，则未开始运行的实例无法启动，已开始运行的实例仍可维持运行至结束。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。

## 数据集成公网流量计费项 {#section_qvr_1d5_hpo .section}

-   计费范围

    数据集成任务运行在公共资源组和独享资源时，所产生的公网流量会按量收取费用，单价为0.8元/GB。

    **说明：** 在产生公网流量的情况下，DataWorks不收取运行在自定义资源组的任务产生的公网流量费用。数据传输过程中产生的其他云产品的公网流量，根据云产品的逻辑为准来决定是否收费。

-   扣费方式

    计费系统会在每小时开始时，计算您前一小时的消耗费用并生成账单，然后从阿里云主账户余额中扣除实际消费的金额。

    例如当前时间是9:30，结算的是8:00~9:00期间产生的费用。

-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用。此时如果您没有购买公共资源调度组资源包，则未开始运行的实例无法启动，已开始运行的实例仍可维持运行至结束。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。

## 数据服务调用次数、执行时间 {#section_754_42t_n0g .section}

-   计费范围

    数据服务的费用由调用次数和执行时间的费用组成，并且每个月会为每个用户提供一定的免费额度。数据服务只会对数据服务API的有效调用次数进行计费，包括数据服务页面进行的在线测试调用。

    -   有效调用：请求响应的errCode为0的请求。
    -   无效调用：请求响应的errCode不为0的请求。
-   计费标准

    |计费项|单位|单价|备注|
    |---|--|--|--|
    |调用次数|百万次|1.33元/百万次|无|
    |执行时间|内存\*秒（GB\*s）|0.00011108元/GB\*s|最小时间单位是100ms，不足100ms则按100ms计算。|

    数据服务每月为每个用户提供免费额度，其中RAM子账号与主账号共享每月的免费额度。

    -   调用次数：每个用户每月调度的前100万次为免费额度。
    -   执行时间：每个用户每月执行的前400000GB\*s为免费额度。
    **说明：** 免费额度在每个自然月开始时清零，重新计算，不会按月累计。

    例如您本月调用了1000万次API，且API分配了2GB内存，每次运行1060ms，则您的费用如下所示。

    -   月度调用次数与费用

        每个月有100万次的调用次数免费额度，所以本月需要计费的调用次数为1000万次-100万次=900万次。每100万次调用次数的价格为1.33元，则本月的月度总调用次数费用为900/100\*1.33=11.97元。

    -   月度执行时间与费用

        执行时间的计量单位为内存（GB）\*秒，即GB\*s。最小时间单位为100ms，不足100ms则按100ms计算。

        您的总执行时间=调用次数\*每次消耗的内存（GB）\*每次运行时间（秒），即10,000,000\*2\*1.1=22,000,000GB\*s。因为每个月有400,000GB\*s的执行时间为免费额度，所以实际需要计费的执行时间为22,000,000-400,000=21,600,000GB\*s。每GB\*s执行时间的价格为0.00011108元，则您本月的总执行时间费用为21,600,000\*0.00011108=2399.33元。

    -   月度总费用

        月度总费用=月度调用次数费用+月度执行时间费用，即11.97+2399.33=2411.3元。

-   扣费方式

    数据服务的计费周期为小时。计费系统会在每小时开始时，计算您前一小时的消耗费用并生成账单，然后从阿里云主账户余额中扣除实际消费的金额。

-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用，此时您将无法正常调用已发布的API。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。
    -   如果结清后再次欠费，则按照新欠费的时间重新延续24小时后停用该服务。

## 数据质量规则实例数量 {#section_a0u_dk2_u5c .section}

-   计费范围

    每个自然日内，通过周期调度实例、补数据实例、试跑触发运行成功的数据质量规则实例，均会纳入计费范围。

-   计费标准（目前0折免费）

    |每日规则实例个数|单价（元/日）|
    |--------|-------|
    |1~10|0.00|
    |11~200|20.00|
    |201~1000|50.00|
    |1001~5000|200.00|

-   扣费方式

    计费系统在每天00:00，清算前一个自然日内运行成功的规则实例数量，并根据上述收费标准中的价格区间进行一次扣费，每次仅扣除一个区间的日费用，不会叠加扣费。

    -   运行成功指规则本身运行成功，由于数据质量问题导致的规则报警或阻塞按运行成功进行计费。
    -   当天数据质量规则实例超过5000后达到按量付费上限，后续规则实例将停止运行。如果需要更大的日调度实例数量，请提交工单联系阿里云技术支持。
-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用，此时您无法启动新的数据质量规则实例，已启动的规则实例不受影响。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。
    -   如果结清后再次欠费，则按照新欠费的时间重新延续24小时后停用该服务。

## 智能监控基线实例数 {#section_2pl_gyi_qo1 .section}

-   计费范围

    所有处于开启状态的基线均会产生基线实例，并根据当天23:59产生的基线实例数量收取费用。

-   计费标准（目前0折免费）

    |每日基线实例数量|单价（元/日）|
    |--------|-------|
    |1~2|0.00|
    |3~10|5.00|
    |11~100|20.00|

-   扣费方式

    计费系统在每天00:00，清算前一个业务日期的基线实例数量，并根据上述收费标准中的价格区间进行一次扣费，每次仅扣除一个区间的日费用，不会叠加扣费。

    -   针对小时任务的小时基线，按照1条基线实例计费。
    -   开启状态的基线数量超过100后达到按量付费上限，将无法生成更多的基线实例。如果需要更大的基线实例数量，请提交工单联系阿里云技术支持。
-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用，此时您无法生成新的基线实例，已启动的基线实例则不受影响。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。如果结清后再次欠费，则按照新欠费的时间重新延续24小时后停用该服务。

## AppStudio开发环境运行空间 {#section_axb_3wg_i0s .section}

-   计费标准

    该计费项按小时收取运行空间（开发环境）的代码调试费用，计费标准如下表所示。

    |运行空间规格（开发环境）|调试费用（元/小时）|
    |------------|----------|
    |1c2g|0.6|
    |2c4g|1.2|
    |4c8g|2.4|
    |8c16g|4.8|

-   扣费方式

    您开始调试时便开始计费，断开调试时便结束计费。

    如果您在调试配置中修改机器规格，修改后调试费用标准按照对应的配置计费。

-   欠费说明

    如果您的账号处于欠费状态，将为您延续24小时的服务时间，并在欠费后的第12小时和第23小时发送通知提醒您尽快续费。

    -   如果欠费状态超过24小时，则该服务会被停用，此时如果您正在调试期间，则当前正在进行的调试不会中断，一旦断开调试便不可重新开始调试。
    -   您在欠费后的24小时内进行充值，则服务不会被停用。
    -   如果结清后再次欠费，则按照新欠费的时间重新延续24小时后停用该服务。

