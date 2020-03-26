# CrossContact  

一款去中心化即时通讯应用 (为了通用的授权和连接，没有围栏的互联网，没有垄断的社交网络)

- 去中心化的CS架构通讯服务，C端可以选择自己想要使用的通讯服务器。同时你也可以搭建自己的通讯服务器。
- 开放的通讯协议
- 名片卡式的社交连接，而不是好友式的强关系。
- 中心化的社交关系链接
- 基于名片卡的开放式的授权服务。
- 标准程序代码开源

## 

###  

#### 1. 去中心化的CS架构通讯服务

应用会提供一个基本的中心化通讯服务器，用户可以默认通过这个服务器收发消息。  
同时用户还可以架设自己的私有服务器，用于提供消息通讯服务。  
例如企业用户，可以在这个应用上架设自己的私有服务器用于消息通讯，服务端自定义自己的消息存贮发送策略，客户端可以在对话中选择使用那个服务器进行消息收发。  
如果通讯双方都选择同一个通讯服务器进行消息通讯，消息将完全通过该服务器中转发送，而默认的中心服务器不参与。  
如果有只有一方选择了私有服务器，则数据的手法规则会遵从私有服务器和公共服务器之间的定义的协议，如是否允许转发，还是无法通讯等。  
**基于这个规则，任何三方都可以将自己的即时通讯服务接入到这个平台。比如某个游戏中的聊天系统，可以完全只需要配置好通讯策略就可以接入聊天服务**  
[更详细的连接规则](component/im_server.md)

#### 2. 开放的通讯协议

**应用层用户消息通讯的协议将开放，并且接受社区提交的新扩展。**

#### 3. 名片卡式的社交连接

人与人之间的社交关系是动态变化和多样的，每个人都有不同的社交圈，同时和每个人的连系也是在不断的变化的。  
比如，认识了新朋友，或者和某些老朋友不再熟络。有或者有了新爱好，进了新公司，有了一个新的圈子。  
目前市面上的通用社交软件如微信基本是一种持久的强关联形式。这也注定了这类社交软件会有存在的生命周期，如QQ被微信取代。  
**本应用使用名片的形式作为用户的凭证**，用户可以创建多张名片，比如公务名片、生活名片、匿名名片、游戏名片等将自己的不同的圈子做隔绝。  
名片作为用户信息的集合和mini版个人主页，名片可以持有多种用户信息，如电话、地址、甚至某些三方社交服务的ID。每个名片可以配置不同的所包含的信息，比如不同的名片使用不同的电话号码。  
**用户之间的连系不是好友关系，而是名片与名片间的连接。同时用户可以改变与其他用户所连接的名片，以应对两者社交关系变化后的连接。**  
比如你可以创建一张公务名片，这张名片可以授权给企业私有服务，比如OA系统等。还可以作为和客户交换的名片，你和客户的连接与你的生活圈是可以进行隔离的。  
同时由于名片机制的存在，为通用的ID授权服务提供了坚实的基础。  

#### 4. 开放式的授权服务

三方可以接入到平台，用户可以将名片授权给三方服务，用于授权登陆。三方可以获取该名片的信息甚至在用户的授权下获取这张名片下的社交关系。  
三方在CrossContact看来也是一个用户，CrossContact提供认证服务。对三方的资质进行认证。在CrossContact中，用户可以在一定程度上自定义自己的用户详情页面，甚至允许提供应用跳转，进入三方的应用或服务。  
三方可以组织自己的好友名片，建立自己的名片关系。  
比如：
> 某个企业，可以创建自己的企业内部名片，新员工和企业交换名片后，企业账号可以对获得的名片进行组织，创建自己的企业架构通讯录，设置不同的通讯、查看权限等。  
> 还可以提供私有通讯服务，让企业的通迅在CrossContact的应用架构下，完全实现通讯的私有化。保证通讯安全。

#### 5. 标准程序代码开源

项目将在进入稳定期后开放源代码作为标准代码，三方可以直接使用项目代码改造成适合自己的通讯服务器，同时在项目初始阶段也会提供一个标准的服务端应用用于快捷的搭建独立的通讯服务器。

## 简易架构图

![简易架构图](img/crosscard.png)
