# 数字人民币商户接入与补贴清算

管理数字人民币商户接入、交易回执、消费补贴、退款和批次清算。

## 参与方与事实

主要参与方包括银行产品运营团队、商户、门店、资金审核人员、清算人员。领域资料记录以下已经确认的事实：

- 多边数字货币桥连接境内外机构
- 数字人民币用于跨境支付和消费场景
- 多地推进县域商户接入与消费活动

## 业务约束

- 商户门店身份
- 终端接入
- 补贴规则版本
- 退款拆分
- 清算对账

`contracts/context.schema.json` 描述资料结构，`fixtures/context.json` 提供不含真实身份信息的示例，`src/digital_yuan_context.py` 负责读取和校验这些资料。

## 开发命令

运行测试：

```bash
python3 -m unittest discover -s tests -v
```

编译检查：

```bash
python3 -m compileall -q src
```

两条命令只读取仓库内文件，不需要连接外部业务系统。
