---
layout: page
title: تواصل معنا
permalink: /contact/
---
<!-- https://medium.com/getform-all-about/how-to-add-a-contact-form-to-your-jekyll-website-6c61e811bdee -->

<form accept-charset="UTF-8" action="https://getform.io/f/1ebf002f-3f03-4db0-9862-25181f55a94d" method="POST" enctype="multipart/form-data" target="_blank">
    <div class="form-group">
        <div class="form-group">
            <label>الأسم</label>
            <input type="text" name="name" class="form-control" required="required">
        </div>
        <label required="required">البريد الإلكتروني</label>
        <input type="email" name="email" class="form-control">
    </div>
    <div class="form-group">
        <label>نوع الرسالة</label>
        <select class="form-control" name="platform" required="required">
            <option>نشر مقال</option>
            <option>إقتراح</option>
            <option>شكوى</option>
            <option>أخرى</option>
        </select>
    </div>
    <hr>
    <div class="form-group mt-3">
        <label>رسالتك</label>
        <br><textarea type="text" name="name" class="form-control" required="required" rows=7></textarea>
    </div>
    <div class="form-group mt-3">
        <label class="mr-2">إرفاق ملف:</label>
        <input type="file" name="file">
    </div>
    <hr>
    <button style="float: left;" type="submit" class="btn btn-secondary">ارسال</button>
</form>