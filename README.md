# 南方科技大学 TIS 教务系统抢课脚本

## 说明

python异步事件循环请求,避免设置超时时间导致的遗漏问题

## 免责声明

- 本脚本（以下简称“脚本”）仅供学习和研究目的，不得用于任何商业或非法活动。使用本脚本进行抢课等活动完全基于用户个人决定，与脚本作者无关。
- 用户在使用本脚本时应确保其行为符合当地法律法规及所在学校的规章制度。脚本作者不对用户使用脚本而可能违反的法律法规或校规负责。
- 使用本脚本可能带来的任何风险（包括但不限于帐号封禁、学校纪律处分等后果）由用户自行承担。脚本作者不承担因使用脚本而产生的任何直接或间接后果的责任。
- 脚本作者不对脚本的持续运作、更新、效果或任何相关服务提供任何形式的保证。脚本的效能可能受到众多因素的影响，包括但不限于网络环境、系统兼容性等。
- 对于本免责声明的解释或适用，脚本作者保留最终解释权。

## 运行环境

- python3

## 依赖库

- aiohttp
- lxml
- pyyaml
- requests

## 用法

- 确保安装了依赖库 (安装指令: `pip install aiohttp lxml pyyaml requests json`)
- 在同级配置文件 **config.yaml** 填写代抢课程(必须),学生 id(必须),密码(必须),tis cookie(可选)
- 运行 py 文件(`python main.py`)
  > 不当的使用行为可能会导柱包括但不限于下列后果:
  >
  > 1. CAS 对身份认证进行 IP 限流
  > 2. TIS 教务系统进行用户层级限流
  > 3. 直接或间接触犯校规及法律法规
