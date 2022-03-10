企业微信HOOK, 企业微信PC版hook

支持获取联系人、群、发消息、群操作、添加好友、收消息等 你可以通过扩展来实现：

监控或收集企业微信消息
自动消息推送
聊天机器人
通过企业微信远程控制你的设备
测试可以使用语言有C/C++，C#，易语言，Python, Java, Go, NodeJs, PHP, VB, Delphi。
支持的版本：3.1.23.6025

java 示例

public final static int 执行结果 = 10002;

public final static int 登录二维码 = 10003;

public final static int 获取内部联系人 = 10103;

public final static int 获取外部联系人 = 10104;

public final static int 获取当前登录帐号的信息 = 11035;

public final static int 手机号查询用户信息 = 10121;

public final static int 通过搜索添加好友 = 10131;

public final static int 获取群组列表 = 10301;

public final static int 获取群组成员列表 = 10302;

public final static int 创建群聊 = 10303;

public final static int 发布群公告 = 10311;

public final static int 接发文本消息 = 10401;

public final static int 接发图片消息 = 10402;

public final static int 接发视频消息 = 10403;

public final static int 接发语音消息 = 10404;

public final static int 接发文件消息 = 10405;

public final static int 接收位置消息 = 10406;

public final static int 发送链接消息 = 10407;

public final static int 接发表情消息 = 10408;

public final static int 接收红包消息 = 10409;

public final static int 接发名片消息 = 10410;

public final static int 发送app消息 = 10411;

public final static int 群内AT人 = 10412;

public final static int 通知消息 = 10499;

/**
 * 获取内部联系人
 *
 * @param clientId
 */
public static void getInnerUsers(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 获取外部联系人
 *
 * @param clientId
 */
public static void getExternalUsers(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 获取群组列表
 *
 * @param clientId
 */
public static void getRooms(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 获取群组列表
 * @param clientId 
 */
public static void getChatRoomMembers(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 发送文字
 * @param clientId 
 * @param json  
 */
public static void sendText(int clientId, String json) { 
    Boolean aa = WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 发送图片
 * @param clientId 
 * @param json  
 */
public static void sendImage(int clientId, String json) { 
    WxWorkInterface.INSTANCE.SendData(clientId, json);
} 

/**
 * 发送文件
 * @param clientId 
 * @param json  
 */
public static void sendFile(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 发送名片
 * @param clientId 
 * @param json  
 */
public static void sendCard(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}

/**
 * 通过搜索添加好友
 * @param clientId 
 * @param json  
 */
public static void addFriend(int clientId, String json) {
    WxWorkInterface.INSTANCE.SendData(clientId, json);
} 

/**
 * 群成员操作
 * @param clientId 
 */
public static void editRoomMember(int clientId, String json) {       
    WxWorkInterface.INSTANCE.SendData(clientId, json);
}  


public static void main(String[] args) {
    //回调
    Boolean aBoolean = WxWorkInterface.INSTANCE.InitCallback(connect, recv, close);
     
    //载入企业微信
    int code = WxWorkInterface.INSTANCE.InjectWxWork(WxWorkInterface.libpathstring, "");
    
    WxWorkInterface.INSTANCE.sendText(clientId,json);
} 
