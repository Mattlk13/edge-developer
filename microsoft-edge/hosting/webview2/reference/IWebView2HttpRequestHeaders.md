---
description: Host web content in your Win32 app with the Microsoft Edge WebView2 control
title: Microsoft Edge WebView2 for Win32 apps
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/09/2019
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, webview, win32 apps, win32, edge
---

# interface IWebView2HttpRequestHeaders 

```
interface IWebView2HttpRequestHeaders
  : public IUnknown
```

HTTP request headers.

## Summary

 Members                        | Descriptions
--------------------------------|---------------------------------------------
[GetHeader](#getheader) | Gets the header value matching the name.
[Contains](#contains) | Checks whether the headers contain an entry matching the header name.
[SetHeader](#setheader) | Adds or updates header that matches the name.
[RemoveHeader](#removeheader) | Removes header that matches the name.
[GetIterator](#getiterator) | Gets an iterator over the collection of request headers.

Used to inspect or modify the HTTP request on WebResourceRequested event and NavigationStarting event.

## Members

#### GetHeader 

Gets the header value matching the name.

> public HRESULT [GetHeader](#getheader)(LPCWSTR name,LPWSTR * value)

#### Contains 

Checks whether the headers contain an entry matching the header name.

> public HRESULT [Contains](#contains)(LPCWSTR name,BOOL * contains)

#### SetHeader 

Adds or updates header that matches the name.

> public HRESULT [SetHeader](#setheader)(LPCWSTR name,LPCWSTR value)

#### RemoveHeader 

Removes header that matches the name.

> public HRESULT [RemoveHeader](#removeheader)(LPCWSTR name)

#### GetIterator 

Gets an iterator over the collection of request headers.

> public HRESULT [GetIterator](#getiterator)([IWebView2HttpHeadersCollectionIterator](IWebView2HttpHeadersCollectionIterator.md#iwebview2httpheaderscollectioniterator) ** iterator)

