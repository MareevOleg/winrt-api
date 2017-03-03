---
-api-id: M:Windows.UI.Text.ITextRange.Copy
-api-type: winrt method
---

<!-- Method syntax
public void Copy()
-->

# Windows.UI.Text.ITextRange.Copy

## -description
Copies the text of the text range to the Clipboard.

## -remarks
> [!NOTE]
> On Windows Phone, this method throws an exception. Programmatic access to the clipboard is not supported on Windows Phone.

The [ITextRange.Cut](itextrange_cut.md), [Copy](itextrange_copy.md), and [Paste](itextrange_paste.md) methods let you perform the usual cut, copy, and paste operations on a text range. The clipboard formats that are typically supported include CF_TEXT and CF_RTF. You can also use private clipboard formats to access text in custom formats.

To copy and replace plain text, you can use the [ITextRange.GetText](itextrange_gettext.md) and [SetText](itextrange_settext.md) methods. To copy formatted text from one range to another without using the Clipboard, you can use the [Copy](itextrange_copy.md) and [Paste](itextrange_paste.md) methods along with the [FormattedText](itextrange_formattedtext.md) property. For example:



```javascript
textRange2.FormattedText = textRange1.FormattedText;

```



## -examples

## -see-also
[ITextRange.Cut](itextrange_cut.md), [ITextRange.Paste](itextrange_paste.md)