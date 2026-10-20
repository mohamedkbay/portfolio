# فوترة · Fawtara

**Invoice capture today; a Flutter financial companion in design.**

[Public source](https://github.com/mohamedkbay/fawtara-public) · [Back to selected work](../README.md)

**Availability:** Browser source available · Flutter, local SQLite, alerts and Qwen remain a design proposal.

## My contribution · دوري

Browser invoice workflow development and a mobile interface/motion proposal for the planned Flutter edition.

تطوير مسار الفواتير في المتصفح وتصميم الواجهة والمعاينة المتحركة لنسخة Flutter المقترحة.

## Mobile direction · design preview

<p align="center"><img src="../assets/fawtara/logo.png" width="72" alt="Proposed Fawtara receipt logo" /></p>

**كل فاتورة، خطوة أوضح.**

![Fawtara mobile concept walkthrough](../assets/fawtara/walkthrough.gif)

[Watch the 43-second walkthrough](../assets/fawtara/walkthrough.mp4) · [Open the full mobile screen](../assets/fawtara/mobile-concept.png)

This is a design and motion proposal with illustrative records, not footage of a completed Flutter application or a live Qwen response.

التصور الجديد لفوترة: تطبيق Flutter، قاعدة بيانات محلية داخل الهاتف، مبالغ وتصنيفات ومواعيد استحقاق، وتنبيهات للمصروفات والفواتير، مع تحليل اختياري عبر Qwen بمفتاح كل مستخدم.

The proposed workflow is capture → enter details → save locally → review spending and due dates → receive local alerts → optionally review and send a summary to Qwen. Financial checks are based on the records the user enters. The existing public browser edition remains available below.

## Existing browser edition · actual interface captures

<p align="center">
<img src="../assets/fawtara/phone-home.jpg" height="480" alt="Fawtara empty invoice archive in the phone layout" />
<img src="../assets/fawtara/phone-add-invoice.jpg" height="480" alt="Fawtara invoice form in the phone layout" />
</p>

**Mobile invoice archive · Add an invoice**

Captured from the actual local web interface using a phone-sized viewport, with an empty archive and blank invoice fields. No customer invoices or account records are shown.

## Overview · الفكرة

Make it easier to capture invoices from a phone and find them later by client, date or notes.

فوترة ينظّم صور الفواتير مع اسم الزبون والتاريخ والملاحظات، ويسهّل البحث والرجوع لها من الهاتف.

## Product scope · نطاق العمل

- Camera capture and gallery uploads, with image compression and previews.
- Invoice records with client names, dates and notes.
- Search, date filters, sorting and full-screen image viewing.
- A responsive interface with a workflow designed around mobile use.

## Technology

React · TypeScript · Material UI · Zustand · Vite

## Availability

The [public browser-only edition](https://github.com/mohamedkbay/fawtara-public) is available as source code. It stores invoice images and details in the current browser's local storage, with no database or remote storage integration to configure. See its README for running and building the application.
