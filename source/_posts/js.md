---
title: 有趣的js
---


`
// 提取URL参数
let url='https://alibaba.com?a-1&b=2&c=3#hash';
function queryURLParams(URL)let url = uRL.split('?')[1];const urlSearchParams =new URlSearchParams(url);const params =0bject.fromEntries(urlSearchParams.entries());
    return params;
console.log(queryURLParams(url));
`