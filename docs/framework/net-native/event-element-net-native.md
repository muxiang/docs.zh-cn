---
title: "&lt;事件&gt;元素 (.NET Native) | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: e53b029c-9d6d-4c0a-9cdc-5cfca8a5ca47
caps.latest.revision: 11
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
caps.handback.revision: 11
---
# &lt;事件&gt;元素 (.NET Native)
将运行时反射策略应用到一个事件。  
  
## <a name="syntax"></a>语法  
  
```xml  
  
<Event Name="event_name"   
       Browse="policy_type"   
       Dynamic="policy_type" />  
  
```  
  
## <a name="attributes-and-elements"></a>特性和元素  
 下列各节描述了特性、子元素和父元素。  
  
### <a name="attributes"></a>特性  
  
|特性|特性类型|描述|  
|---------------|--------------------|-----------------|  
|`Name`|常规|必需的特性。 指定事件名称。|  
|`Browse`|映像|可选特性。 控制对该事件信息的查询或列举该事件，但并不在运行时间启用任何动态访问。|  
|`Dynamic`|映像|可选特性。 控制运行时对该事件的访问，以启用动态编程。 该策略确保一个事件可在运行时间内得到处理。|  
  
## <a name="name-attribute"></a>Name 特性  
  
|值|说明|  
|-----------|-----------------|  
|*method_name*|事件名称。 该事件的类型定义由容器的父[ <> \> ](../../../docs/framework/net-native/type-element-net-native.md)或[ <> \> ](../../../docs/framework/net-native/typeinstantiation-element-net-native.md)元素。|  
  
## <a name="all-other-attributes"></a>所有其他特性  
  
|值|说明|  
|-----------|-----------------|  
|*policy_setting*|该设置将应用到这个事件的策略类型。 可能值为 `Auto`、`Excluded`、`Included` 和 `Required`。 有关详细信息，请参阅[运行时指令策略设置](../../../docs/framework/net-native/runtime-directive-policy-settings.md)。|  
  
### <a name="child-elements"></a>子元素  
 无。  
  
### <a name="parent-elements"></a>父元素  
  
|元素|描述|  
|-------------|-----------------|  
|[<>\>](../../../docs/framework/net-native/type-element-net-native.md)|将反射策略应用到一种类型及其所有成员。|  
|[<>\>](../../../docs/framework/net-native/typeinstantiation-element-net-native.md)|将反射策略应用到一种构造泛型类型及其所有成员。|  
  
## <a name="remarks"></a>备注  
 如果一个事件的策略没有得到显式定义，它将继承其父元素的运行时策略。  
  
## <a name="see-also"></a>另请参阅  
 [运行时指令 (rd.xml) 配置文件引用](../../../docs/framework/net-native/runtime-directives-rd-xml-configuration-file-reference.md)   
 [运行时指令元素](../../../docs/framework/net-native/runtime-directive-elements.md)   
 [运行时指令策略设置](../../../docs/framework/net-native/runtime-directive-policy-settings.md)