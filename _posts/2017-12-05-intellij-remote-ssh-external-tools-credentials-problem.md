---
layout: post
title: "IntelliJ IDE 의 Remote SSH External Tools 에서 Credentials 안 뜰때 확인할 사항"
date: 2017-12-05 11:23:00 +0900
---

IntelliJ 계열 IDE에서 Remote SSH External Tools 사용할 때, 설정된 Credentials가 하나도 뜨지 않는 경우가 있다. 아래의 이미지 처럼 말이다.



<amp-img layout="responsive" src="http://note.minbyul.com/assets/images/intellij_remote_ssh_external_tools_0.png"></amp-img>



불편을 감수하고 쓸 때마다 credentials 설정을 해 줘야 하나? 그럴리가 없는데.. 라고 생각하며 계속 인터넷을 뒤지다가 결국 원인을 찾았다.



<amp-img layout="responsive" src="http://note.minbyul.com/assets/images/intellij_remote_ssh_external_tools_0-1.png"></amp-img>

위 이미지의 본문은 <https://www.jetbrains.com/help/phpstorm/creating-a-remote-server-configuration.html> 에서도 확인이 가능하다.



<amp-img layout="responsive" src="http://note.minbyul.com/assets/images/intellij_remote_ssh_external_tools_1.png"></amp-img>

위 이미지처럼 **Visible only for this project** 체크박스의 체크가 해제된 상태로 두면 된다.



다시 원하는 Remote SSH External Tools를 실행해 보자.



<amp-img layout="responsive" src="http://note.minbyul.com/assets/images/intellij_remote_ssh_external_tools_2.png"></amp-img>

위 이미지처럼 이제 Credentials가 제대로 뜨는 것을 확인할 수 있다.

