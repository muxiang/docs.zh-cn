---
title: 如何：使用设计器禁用 ToolStripMenuItem
ms.date: 03/30/2017
helpviewer_keywords:
- ToolStripMenuItems [Windows Forms], disabling in designer
- MenuStrip control [Windows Forms], disabling menu items in designer
- menu items [Windows Forms], disabling
- menus [Windows Forms], disabling items
ms.assetid: 985e311e-7d67-4205-b5a3-d045b68a4a03
ms.openlocfilehash: 3ce18d40910145a076cc7084e2fba8ee0229c21f
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33531549"
---
# <a name="how-to-disable-toolstripmenuitems-using-the-designer"></a>如何：使用设计器禁用 ToolStripMenuItem
你可以限制或扩大用户可通过启用和禁用菜单项以响应用户活动的命令。 当创建，但这可以通过调整时，默认情况下启用菜单项<xref:System.Windows.Forms.ToolStripMenuItem.Enabled%2A>属性。 在设计时使用此属性可**属性**窗口或以编程方式通过在代码中设置。 有关详细信息，请参阅[如何： 禁用 ToolStripMenuItems](../../../../docs/framework/winforms/controls/how-to-disable-toolstripmenuitems.md)。  
  
> [!NOTE]
>  显示的对话框和菜单命令可能会与“帮助”中的描述不同，具体取决于你现用的设置或版本。 若要更改设置，请在 **“工具”** 菜单上选择 **“导入和导出设置”** 。 有关详细信息，请参阅[在 Visual Studio 中自定义开发设置](http://msdn.microsoft.com/library/22c4debb-4e31-47a8-8f19-16f328d7dcd3)。  
  
### <a name="to-disable-a-menu-item-at-design-time"></a>若要在设计时禁用菜单项  
  
1.  选择窗体上的菜单项，其中设置<xref:System.Windows.Forms.ToolStripMenuItem.Enabled%2A>属性`false`。  
  
    > [!TIP]
    >  禁用菜单中的第一个或顶级菜单项将禁用菜单中包含的所有菜单项。 同样，禁用菜单项具有子菜单项将禁用这些子菜单项。 如果给定的菜单上的所有命令都都向用户不可用，它则被视为良好编程习惯隐藏和禁用整个菜单上，这会带来全新的用户界面。 你应同时隐藏和禁用菜单上，因为仅靠隐藏不会向菜单命令的快捷键通过阻止访问。 设置<xref:System.Windows.Forms.ToolStripItem.Visible%2A>顶级菜单项的属性`false`若要隐藏整个菜单。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.Forms.MenuStrip>  
 <xref:System.Windows.Forms.ToolStripMenuItem>  
 [如何：隐藏 ToolStripMenuItem](../../../../docs/framework/winforms/controls/how-to-hide-toolstripmenuitems.md)  
 [MenuStrip 控件概述](../../../../docs/framework/winforms/controls/menustrip-control-overview-windows-forms.md)
