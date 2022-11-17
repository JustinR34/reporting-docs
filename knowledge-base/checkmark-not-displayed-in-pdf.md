---
title: CheckMark Symbol Not Displayed in PDF
description: CheckMark symbol appears as an empty box in PDF
type: how-to
page_title: Display CheckMark in PDF Report
slug: checkmark-not-displayed-in-pdf
position: 
tags: 
ticketid: 1587424
res_type: kb
---

## Environment
<table>
	<tbody>
		<tr>
			<td>Product</td>
			<td>Progress® Telerik® Reporting</td>
		</tr>
	</tbody>
</table>


## Description
I cannot get the checkmark symbol to be displayed in the PDF report document. It looks fine in the Preview of the designer. When generating a PDF it turns the checkmark into an empty box.

## Solution
Here is a list of fonts that support the checkmark - [CHECK MARK (U+2713) Font Support](https://www.fileformat.info/info/unicode/char/2713/fontsupport.htm).

For example, the __Arial Unicode MS__ is in the list and the PDF document displays the '✓' character correctly when the report item that contains it is styled to use this font.

You need to set the Font of the Report or the report item that contains the checkmark to one that is in the above list.
