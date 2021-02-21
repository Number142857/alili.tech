---
title: Session
hidden: true
categories: [reprint]
slug: 1ff9ec48
date: 2018-11-04 02:30:10
---

{{< raw >}}
<h1 id="articleHeader0">Session</h1><h2 id="articleHeader1">Cookie &#x548C; Session</h2><h3 id="articleHeader2">&#x533A;&#x522B;&#x4E0E;&#x8054;&#x7CFB;</h3><ol><li>&#x7531;&#x4E8E;HTTP&#x534F;&#x8BAE;&#x662F;&#x65E0;&#x72B6;&#x6001;&#x7684;&#x534F;&#x8BAE;&#xFF0C;&#x6240;&#x4EE5;&#x670D;&#x52A1;&#x7AEF;&#x9700;&#x8981;&#x8BB0;&#x5F55;&#x7528;&#x6237;&#x7684;&#x72B6;&#x6001;&#x65F6;&#xFF0C;&#x5C31;&#x9700;&#x8981;&#x7528;&#x67D0;&#x79CD;&#x673A;&#x5236;&#x6765;&#x8BC6;&#x5177;&#x4F53;&#x7684;&#x7528;&#x6237;&#xFF0C;&#x8FD9;&#x4E2A;&#x673A;&#x5236;&#x5C31;&#x662F;<strong>Session</strong>&#x3002;<br>&#x5178;&#x578B;&#x7684;&#x573A;&#x666F;&#x6BD4;&#x5982;<strong>&#x8D2D;&#x7269;&#x8F66;</strong>&#xFF0C;&#x5F53;&#x4F60;&#x70B9;&#x51FB;&#x4E0B;&#x5355;&#x6309;&#x94AE;&#x65F6;&#xFF0C;&#x7531;&#x4E8E;HTTP&#x534F;&#x8BAE;&#x65E0;&#x72B6;&#x6001;&#xFF0C;&#x6240;&#x4EE5;&#x5E76;&#x4E0D;&#x77E5;&#x9053;&#x662F;&#x54EA;&#x4E2A;&#x7528;&#x6237;&#x64CD;&#x4F5C;&#x7684;&#xFF0C;&#x6240;&#x4EE5;&#x670D;&#x52A1;&#x7AEF;&#x8981;&#x4E3A;&#x7279;&#x5B9A;&#x7684;&#x7528;&#x6237;&#x521B;&#x5EFA;&#x4E86;&#x7279;&#x5B9A;&#x7684;Session&#xFF0C;&#x7528;&#x7528;&#x4E8E;<strong>&#x6807;&#x8BC6;&#x8FD9;&#x4E2A;&#x7528;&#x6237;</strong>&#xFF0C;<strong>&#x5E76;&#x4E14;&#x8DDF;&#x8E2A;&#x7528;&#x6237;</strong>&#xFF0C;&#x8FD9;&#x6837;&#x624D;&#x77E5;&#x9053;&#x8D2D;&#x7269;&#x8F66;&#x91CC;&#x9762;&#x6709;&#x51E0;&#x4EF6;&#x7269;&#x54C1;&#x3002;&#x8FD9;&#x4E2A;Session&#x662F;<strong>&#x4FDD;&#x5B58;&#x5728;&#x670D;&#x52A1;&#x7AEF;</strong>&#x7684;&#xFF0C;&#x6709;&#x4E00;&#x4E2A;&#x552F;&#x4E00;&#x6807;&#x8BC6;&#x3002;&#x5728;&#x670D;&#x52A1;&#x7AEF;&#x4FDD;&#x5B58;Session&#x7684;&#x65B9;&#x6CD5;&#x5F88;&#x591A;&#xFF0C;&#x5185;&#x5B58;&#x3001;&#x6570;&#x636E;&#x5E93;&#x3001;&#x6587;&#x4EF6;&#x3001;&#x96C6;&#x7FA4;&#x7B49;&#x3002;</li><li>&#x670D;&#x52A1;&#x7AEF;&#x5982;&#x4F55;&#x8BC6;&#x522B;&#x7279;&#x5B9A;&#x7684;&#x5BA2;&#x6237;&#xFF1F;&#x7B2C;&#x4E00;&#x6B21;&#x521B;&#x5EFA;Session&#x7684;&#x65F6;&#x5019;&#xFF0C;&#x670D;&#x52A1;&#x7AEF;&#x4F1A;&#x5728;HTTP&#x534F;&#x8BAE;&#x4E2D;&#x544A;&#x8BC9;&#x5BA2;&#x6237;&#x7AEF;&#xFF0C;&#x9700;&#x8981;<strong>&#x5728; Cookie &#x91CC;&#x9762;&#x8BB0;&#x5F55;&#x4E00;&#x4E2A;Session ID</strong>&#xFF0C;&#x4EE5;&#x540E;<strong>&#x6BCF;&#x6B21;&#x8BF7;&#x6C42;</strong>&#x628A;&#x8FD9;&#x4E2A;&#x4F1A;&#x8BDD;ID&#x53D1;&#x9001;&#x5230;&#x670D;&#x52A1;&#x5668;&#xFF0C;&#x5C31;&#x53EF;&#x4EE5;&#x4F9D;&#x636E;&#x6B64;&#x6765;&#x8BC6;&#x522B;&#x4E0D;&#x540C;&#x5BA2;&#x6237;&#x7AEF;&#x4E86;&#x3002;<br>&#x5982;&#x679C;&#x5BA2;&#x6237;&#x7AEF;&#x7684;&#x6D4F;&#x89C8;&#x5668;&#x7981;&#x7528;&#x4E86; Cookie &#x600E;&#x4E48;&#x529E;&#xFF1F;&#x4E00;&#x822C;&#x8FD9;&#x79CD;&#x60C5;&#x51B5;&#x4E0B;&#xFF0C;&#x4F1A;&#x4F7F;&#x7528;&#x4E00;&#x79CD;&#x53EB;&#x505A;<strong>URL&#x91CD;&#x5199;</strong>&#x7684;&#x6280;&#x672F;&#x6765;&#x8FDB;&#x884C;&#x4F1A;&#x8BDD;&#x8DDF;&#x8E2A;&#xFF0C;&#x5373;&#x6BCF;&#x6B21;HTTP&#x4EA4;&#x4E92;&#xFF0C;URL&#x540E;&#x9762;&#x90FD;&#x4F1A;&#x88AB;&#x9644;&#x52A0;&#x4E0A;&#x4E00;&#x4E2A;&#x8BF8;&#x5982; sid=xxxxx &#x8FD9;&#x6837;&#x7684;&#x53C2;&#x6570;&#xFF0C;&#x670D;&#x52A1;&#x7AEF;&#x636E;&#x6B64;&#x6765;&#x8BC6;&#x522B;&#x7528;&#x6237;&#x3002;</li></ol><p>&#x603B;&#x7ED3;:</p><ol><li>Session&#x662F;&#x5728;<strong>&#x670D;&#x52A1;&#x7AEF;</strong>&#x4FDD;&#x5B58;&#x7684;&#x4E00;&#x4E2A;<strong>&#x6570;&#x636E;&#x7ED3;&#x6784;</strong>&#xFF0C;&#x7528;&#x6765;<strong>&#x8DDF;&#x8E2A;&#x7528;&#x6237;&#x7684;&#x72B6;&#x6001;</strong>&#xFF0C;&#x8FD9;&#x4E2A;&#x6570;&#x636E;&#x53EF;&#x4EE5;&#x4FDD;&#x5B58;&#x5728;&#x96C6;&#x7FA4;&#x3001;&#x6570;&#x636E;&#x5E93;&#x3001;&#x6587;&#x4EF6;&#x4E2D;&#xFF1B;</li><li>Cookie&#x662F;<strong>&#x5BA2;&#x6237;&#x7AEF;</strong>&#x4FDD;&#x5B58;&#x7528;&#x6237;&#x4FE1;&#x606F;&#x7684;&#x4E00;&#x79CD;&#x673A;&#x5236;&#xFF0C;&#x7528;&#x6765;&#x8BB0;&#x5F55;&#x7528;&#x6237;&#x7684;&#x4E00;&#x4E9B;&#x4FE1;&#x606F;&#xFF0C;&#x4E5F;&#x662F;<strong>&#x5B9E;&#x73B0;Session&#x7684;&#x4E00;&#x79CD;&#x65B9;&#x5F0F;</strong>&#x3002;</li></ol><p>&#x6765;&#x6E90;&#x94FE;&#x63A5;&#xFF1A;<a href="https://www.zhihu.com/question/19786827/answer/28752144" rel="nofollow noreferrer" target="_blank">https://www.zhihu.com/questio...</a></p><h4>&#x4EC0;&#x4E48;&#x662F;session&#xFF1F;</h4><ol><li>&#x670D;&#x52A1;&#x5668;&#x901A;&#x8FC7;Cookie&#x53D1;&#x9001;&#x7ED9;&#x5BA2;&#x6237;&#x7AEF;&#x4E00;&#x4E2A;sessionID</li><li>sessionID&#x5BF9;&#x5E94;&#x670D;&#x52A1;&#x5668;&#x91CC;&#x7684;&#x4E00;&#x5C0F;&#x5757;&#x5185;&#x5B58;&#xFF0C;&#x8FD9;&#x91CC;&#x4FDD;&#x5B58;&#x7740;&#x7528;&#x6237;&#x7684;&#x4FE1;&#x606F;&#xFF0C;&#x4F8B;&#x5982;&#x767B;&#x5F55;&#x4FE1;&#x606F;&#xFF0C;&#x8D2D;&#x7269;&#x8F66;&#x4FE1;&#x606F;&#x7B49;&#x3002;</li><li>&#x6BCF;&#x6B21;&#x7528;&#x6237;&#x8BBF;&#x95EE;&#x670D;&#x52A1;&#x5668;&#x7684;&#x65F6;&#x5019;&#xFF0C;&#x670D;&#x52A1;&#x5668;&#x901A;&#x8FC7;&#x6D4F;&#x89C8;&#x5668;&#x53D1;&#x9001;&#x6765;&#x7684;cookie&#x91CC;&#x7684;sessionID&#x53BB;&#x8BFB;&#x53D6;&#x5BF9;&#x5E94;&#x7684;&#x5185;&#x5B58;&#x91CC;&#x7684;&#x4FE1;&#x606F;&#xFF0C;&#x4EE5;&#x6B64;&#x6765;&#x77E5;&#x9053;&#x7528;&#x6237;&#x7684;&#x9690;&#x79C1;&#x4FE1;&#x606F;&#x3002;</li></ol><h4>&#x6CE8;&#x610F;</h4><ol><li>session&#x7684;&#x597D;&#x5904;&#x662F;&#x9632;&#x6B62;&#x7528;&#x6237;&#x968F;&#x610F;&#x7BE1;&#x6539;cookie&#xFF0C;&#x83B7;&#x53D6;&#x522B;&#x4EBA;&#x7684;&#x4FE1;&#x606F;&#x3002;</li><li>&#x5982;&#x679C;&#x7528;&#x6237;&#x968F;&#x610F;&#x7BE1;&#x6539;&#x4E86;sessionID&#xFF0C;&#x90A3;&#x4E48;&#x53EA;&#x80FD;&#x91CD;&#x65B0;&#x767B;&#x5F55;&#x3002;</li><li>&#x56E0;&#x4E3A;sessionID&#x662F;&#x968F;&#x673A;&#x6570;&#xFF0C;&#x6216;&#x8005;&#x968F;&#x673A;&#x6570;&#x5939;&#x6742;&#x7740;&#x4E00;&#x4E9B;&#x5B57;&#x6BCD;&#xFF0C;&#x6240;&#x4EE5;&#x6CA1;&#x6709;&#x53EF;&#x80FD;&#x66B4;&#x529B;&#x7834;&#x89E3;sessionID&#xFF0C;&#x83B7;&#x53D6;&#x522B;&#x7684;&#x7528;&#x6237;&#x7684;&#x4FE1;&#x606F;&#x3002;</li></ol><p><span class="img-wrap"><img data-src="/img/bVbib4H?w=959&amp;h=552" src="https://static.alili.tech/img/bVbib4H?w=959&amp;h=552" alt="clipboard.png" title="clipboard.png" style="cursor:pointer;display:inline"></span></p><p>&#x7C7B;&#x6BD4;&#xFF1A;session&#x76F8;&#x5F53;&#x4E8E;&#x53D1;&#x4F1A;&#x5458;&#x5361;&#xFF0C;&#x4F1A;&#x5458;&#x5361;&#x4E0A;&#x53EA;&#x6709;&#x5361;&#x53F7;&#xFF08;sessionID&#xFF09;&#x3002;&#x4E0B;&#x6B21;&#x53BB;&#x5065;&#x8EAB;&#x623F;&#x7684;&#x65F6;&#x5019;&#xFF0C;&#x53EA;&#x8981;&#x770B;&#x5361;&#x53F7;&#x4E0A;&#xFF0C;&#x5C31;&#x80FD;&#x786E;&#x5B9A;&#x4F60;&#x672C;&#x4EBA;&#x7684;&#x53BB;&#x4ED6;&#x4FE1;&#x606F;&#x3002;<br>&#x800C;cookie&#x76F8;&#x5F53;&#x4E8E;&#x628A;&#x4FE1;&#x606F;&#x90FD;&#x5199;&#x5728;&#x4F1A;&#x5458;&#x5361;&#x4E0A;&#x4E86;&#x3002;</p><p><a href="https://github.com/mtt3366/CookieStudy/commit/27a2dace608d1b42652763684f4e74e6a5c386b1" rel="nofollow noreferrer" target="_blank">&#x5173;&#x4E8E;session&#x7684;&#x5B9E;&#x73B0;&#x4EE3;&#x7801;&#x6F14;&#x793A;&#xFF08;nodejs&#xFF09;</a></p><h2 id="articleHeader3">&#x603B;&#x7ED3;</h2><h3 id="articleHeader4">Session &#x4E0E; Cookie &#x7684;&#x5173;&#x7CFB;</h3><p>&#x4E00;&#x822C;&#x6765;&#x8BF4;&#xFF0C;Session &#x57FA;&#x4E8E; Cookie &#x6765;&#x5B9E;&#x73B0;&#x3002;</p><h3 id="articleHeader5">Cookie</h3><ol><li>&#x670D;&#x52A1;&#x5668;&#x901A;&#x8FC7; <code>Set-Cookie</code> &#x5934;&#x7ED9;&#x5BA2;&#x6237;&#x7AEF;&#x4E00;&#x4E32;&#x5B57;&#x7B26;&#x4E32;</li><li>&#x5BA2;&#x6237;&#x7AEF;&#x6BCF;&#x6B21;&#x8BBF;&#x95EE;&#x76F8;&#x540C;&#x57DF;&#x540D;&#x7684;&#x7F51;&#x9875;&#x65F6;&#xFF0C;&#x5FC5;&#x987B;&#x5E26;&#x4E0A;&#x8FD9;&#x6BB5;&#x5B57;&#x7B26;&#x4E32;</li><li>&#x5BA2;&#x6237;&#x7AEF;&#x8981;&#x5728;&#x4E00;&#x6BB5;&#x65F6;&#x95F4;&#x5185;&#x4FDD;&#x5B58;&#x8FD9;&#x4E2A;Cookie</li><li>Cookie &#x9ED8;&#x8BA4;&#x5728;&#x7528;&#x6237;&#x5173;&#x95ED;&#x9875;&#x9762;&#x540E;&#x5C31;&#x5931;&#x6548;&#xFF0C;&#x540E;&#x53F0;&#x4EE3;&#x7801;&#x53EF;&#x4EE5;&#x4EFB;&#x610F;&#x8BBE;&#x7F6E; Cookie &#x7684;&#x8FC7;&#x671F;&#x65F6;&#x95F4;</li><li>&#x5927;&#x5C0F;&#x5927;&#x6982;&#x5728; 4kb &#x4EE5;&#x5185;</li></ol><h3 id="articleHeader6">Session</h3><p>Session&#xFF08;&#x4E0D;&#x7FFB;&#x8BD1;,&#x6216;&#x7FFB;&#x8BD1;&#x4E3A;&#x4F1A;&#x8BDD;&#xFF09;</p><ol><li>&#x5C06; SessionID&#xFF08;&#x968F;&#x673A;&#x6570;&#xFF09;&#x901A;&#x8FC7; Cookie &#x53D1;&#x7ED9;&#x5BA2;&#x6237;&#x7AEF;</li><li>&#x5BA2;&#x6237;&#x7AEF;&#x8BBF;&#x95EE;&#x670D;&#x52A1;&#x5668;&#x65F6;&#xFF0C;&#x670D;&#x52A1;&#x5668;&#x8BFB;&#x53D6; SessionID</li><li>&#x670D;&#x52A1;&#x5668;&#x6709;&#x4E00;&#x5757;&#x5185;&#x5B58;&#xFF08;&#x54C8;&#x5E0C;&#x8868;&#xFF09;&#x4FDD;&#x5B58;&#x4E86;&#x6240;&#x6709; session</li><li>&#x901A;&#x8FC7; SessionID &#x6211;&#x4EEC;&#x53EF;&#x4EE5;&#x5F97;&#x5230;&#x5BF9;&#x5E94;&#x7528;&#x6237;&#x7684;&#x9690;&#x79C1;&#x4FE1;&#x606F;&#xFF0C;&#x5982; id&#x3001;email</li><li>&#x8FD9;&#x5757;&#x5185;&#x5B58;&#xFF08;&#x54C8;&#x5E0C;&#x8868;&#xFF09;&#x5C31;&#x662F;&#x670D;&#x52A1;&#x5668;&#x4E0A;&#x7684;&#x6240;&#x6709; session</li></ol>
{{< /raw >}}

# 版权声明
本文资源来源互联网，仅供学习研究使用，版权归该资源的合法拥有者所有，

本文仅用于学习、研究和交流目的。转载请注明出处、完整链接以及原作者。 

原作者若认为本站侵犯了您的版权，请联系我们，我们会立即删除！

## 原文标题
Session

## 原文链接
[https://segmentfault.com/a/1190000016692936](https://segmentfault.com/a/1190000016692936)
