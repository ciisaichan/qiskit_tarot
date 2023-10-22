# qiskit_tarot
使用量子计算机抽取卡罗牌

**Note: 此项目只是为了探索量子计算机的应用~~以及好玩~~，不建议大规模使用以免造成算力浪费。**

大致原理以及流程：
1. 使用5个量子比特，随机量子电路
2. 提交至量子计算机
3. 获得5个量子比特的观测统计结果
4. 将概率最高的结果的二进制数转为十进制
5. 将十进制结果范围从0-31映射至0-21（塔罗牌牌数范围）
6. 取得对应编号的卡罗牌
7. 通过统计结果数判断奇偶数（奇数为正位、偶数为逆位）
