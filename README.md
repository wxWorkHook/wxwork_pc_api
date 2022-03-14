## 企业微信HOOK, 企业微信PC版hook

支持获取联系人、群、发消息、群操作、添加好友、收消息等 你可以通过扩展来实现：

监控或收集企业微信消息
自动消息推送
聊天机器人
通过企业微信远程控制你的设备
测试可以使用语言有C/C++，C#，易语言，Python, Java, Go, NodeJs, PHP, VB, Delphi。
支持的版本：3.1.22 

## h2功能清单

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

## 示例

    /**
     * 发送图片
     * @param iClientId
     * @param conversation_id 接收者的会话ID
     * @param file 文件路径
     */
    public static void sendImage(int iClientId, String json) { 
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }

    /**
     * 发送视频
     * @param iClientId
     * @param conversation_id 接收者的会话ID
     * @param file 文件路径
     */
    public static void sendVideo(int iClientId, String jsone) {
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }

    /**
     * 发送文件
     * @param iClientId
     * @param conversation_id 接收者的会话ID
     * @param file 文件路径
     */
    public static void sendFile(int iClientId, String json) {
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }

    /**
     * 发送名片
     * @param iClientId
     * @param conversation_id 接收者的会话ID
     * @param user_id 用户ID
     */
    public static void sendPersonCard(int iClientId, String json) {
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }

    /**
     * 通过搜索添加好友
     * @param iClientId
     * @param user_id 通过查询获取到的user_id
     * @param v1 通过查询获取到的v1
     * @param verify 验证消息
     */
    public static void addFriend(int iClientId, String json) {
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }

    /**
     * 发送小程序
     * @param iClientId
     * @param json 先发个小程序给机器人，保存json参数传进来就行了。最后一个type参数固定为 11065
     */
    public static void sendApp(int iClientId, String json) {
        WxWorkInterface.INSTANCE.SendData(iClientId, json);
    }
    
    
QQ：1307904544
verify：wxWork
