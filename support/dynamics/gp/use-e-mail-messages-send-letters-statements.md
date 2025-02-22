---
title: Use e-mail messages to send letters, statements, and invoices
description: This article describes how to set up a query and use it to send letters, statements, and invoices by using e-mail messages.
ms.reviewer: 
ms.topic: how-to
ms.date: 03/31/2021
---
# Use e-mail messages to send letters, statements, and invoices to customers in Microsoft Dynamics GP

This article describes how to set up a query and use it to send letters, statements, and invoices by using e-mail messages.

_Applies to:_ &nbsp; Microsoft Dynamics GP  
_Original KB number:_ &nbsp; 903690

## Introduction

This article describes how to use e-mail messages to send letters, statements, and invoices to many customers in Microsoft Dynamics GP and in Microsoft Business Solutions - Great Plains 8.0. You can set up a query and then use the query to send these items.

## More information

To use e-mail messages to send letters, statements, and invoices, follow these steps:

1. Create a letter, statement, or invoice.

   > [!NOTE]
   > If you intend to send letters, statements, or invoices in Portable Document Format (PDF), Adobe Acrobat and Adobe Reader must be installed.

2. Set up Microsoft Dynamics GP to send e-mail messages to the status recipient. To do this, follow these steps:

   1. In Microsoft Dynamics GP 10.0, point to **Tools** on the **Microsoft Dynamics GP** menu, point to **Setup**, point to **Sales**, and then click **Receivables**.

      In Microsoft Dynamics GP 9.0 and in Microsoft Business Solutions - Great Plains 8.0, point to **Setup** on the **Tools** menu, point to **Sales**, and then click **Receivables**.

   2. In the Receivables Management Setup window, enter an e-mail address in the **Status Recipient** box, and then click **OK**.

      > [!NOTE]
      > This e-mail address belongs to the person who will use e-mail messages to send statements to customers.

   3. Point to **Sales** on the **Cards** menu, and then click **Customer**. In the **Customer ID** field, type a customer ID.
   4. In the Customer Maintenance window, click **Options**.
   5. In the Customer Maintenance Options window, click to select the **Send E-mail Statements** check box, and then enter an e-mail address in the **To** box. The **CC** and **BCC** boxes are optional.
   6. Click **OK**.

3. Set up a query for all customers. To do this, follow these steps:  (In GP 2013 and later versions, you need to purchase and install 'Collections Management' to do build queries and query letters. This is a third-party add-on product.)

   1. Point to **Sales** on the **Transactions** menu, and then click **Build Query**.
   2. In the Collections Management Build Query window, enter the required information in the **Query ID** and **Description** boxes.
   3. On the **Customer** tab, click to select the type of query in the **Customer** box, and then select the range by using the **From** and the **To** boxes.

      For example, if you want to select all customers, click to select the first customer in the **From** box, and then click to select the last customer in the **To** box.

   4. Click **Insert** to insert the range.
   5. Repeat steps 2a through step 2d if you want to add other ranges for this query.
   6. Click **Save**.

4. Use the query to send the letters, statements, or invoices. To do this, follow these steps:

   1. Point to **Sales** on the **Transactions** menu, and then click **Query Letters**.
   2. Click to select one or more of the following check boxes:

      - Print Letters
      - Print Statements
      - Print Invoices

   3. Click **Print**.
   4. In the Collections Management Query Actions window, click **Email**. The third-party products that this article discusses are manufactured by companies that are independent of Microsoft. Microsoft makes no warranty, implied or otherwise, regarding the performance or reliability of these products.
