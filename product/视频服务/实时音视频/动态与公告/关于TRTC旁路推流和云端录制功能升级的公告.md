自2022年07月20日起，实时音视频（TRTC）将对当前的 [旁路推流](https://cloud.tencent.com/document/product/647/16826) 功能和 [云端录制](https://cloud.tencent.com/document/product/647/16823) 功能现将进行升级改造，将提升其可用性，助力客户业务更好的开展，升级详情请见下文。

## 旁路转推

原旁路推流功能现升级为旁路转推，在之前功能基础之上支持切换推流域名，即原默认推流域名（`xxxx.livepush.myqcloud.com/xxx.tlivecloud.com`）支持切换您在云直播控制台绑定的推流域名，如需切换，请先前往 [云直播控制台](https://console.cloud.tencent.com/live/domainmanage) 进行绑定推流域名，并保持推流域名可用，具体操作请参见  [旁路推流配置](https://tcloud-doc.isd.com/document/product/647/50768?!preview#.E6.97.81.E8.B7.AF.E6.8E.A8.E6.B5.81.E9.85.8D.E7.BD.AE)。

>!
>- 推流域名切换前，请先确认您当前推流域名绑定的云直播相关模板（录制、截图鉴黄、水印等），并将其绑定在您即将切换的新域名上，切换域名后，原推流域名上绑定的模板将失效。
>- 切换推流域名生效时间约30分钟，生效后的音视频将按照新推流域名转推至云直播，本次旁路转推功能升级只做底层能力的升级，不涉及您原业务代码的改动。

## 云端录制
TRTC推出全新云端录制功能，更灵活的录制任务管理方式，支持单流和混流录制，支持手动自定义录制和全局自动录制，无需依赖旁路转推功能至云直播，使用TRTC内部服务完成录制功能并存储至云点播。

为了兼容当前客户部分应用正在使用 [旧版云端录制](https://cloud.tencent.com/document/product/647/16823) 的情况，故会针对2022年07月20号发布此次功能前，已经在使用旁路转推功能的应用（SDKAppID 维度，非账号维度）保持当前旧版云端录制功能，其余已创建但未使用旁路转推的应用和2022年07月20日之后新创建的应用将升级为新版云端录制，同时支持旧版云端录制能力切换为新版且不支持回退（同一个应用仅可使用一种录制能力）。

>!
>- 本次录制能力升级不会影响您正在使用中的录制功能，若您当前项目应用使用的是旧版云端录制，我们提供了升级为新版云端录制能力的方式，具体切换方式请关注近期发布的新版云端录制说明文档（将于2022年07月20对外）。
>- 新版云端录制收费详情请请参见 [云端录制计费说明](https://cloud.tencent.com/document/product/647/75047)。



