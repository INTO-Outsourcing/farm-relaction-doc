## 邀请下级送土地合约

- 邀请合约地址（714测试网）：0x03a6D372D89455888928A27904256F2A90E4F7E1

#### 设置层级是1的用户地址

- function adminSetEnv( address landAddress, address initInviter, uint256 maxLand ) public
- 参数
    - landAddress 土地合约地址
    - initInviter 层级是1的用户地址（设置顶层用户地址）
    - maxLand 邀请下级上级最多赠送几块土地

#### 绑定邀请关系

- function bind(address inviter) public
- 参数
    - inviter 上级用户地址

#### 获取某用户邀请的所有下级

- function getInviteeList( address inviter)
- 参数
    - inviter 上级用户地址