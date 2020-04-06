---
layout: page
title: تواصل معنا
permalink: /contact/
---
<!-- https://medium.com/getform-all-about/how-to-add-a-contact-form-to-your-jekyll-website-6c61e811bdee -->

<form accept-charset="UTF-8" action="https://getform.io/f/1ebf002f-3f03-4db0-9862-25181f55a94d" method="POST" enctype="multipart/form-data" target="_blank">
<div class="form-box">
    <div class="form-group">
        <div class="form-group">
            <label>الأسم:</label>
            <input type="text" name="name" class="form-control" required="required">
        </div>
        <label required="required">البريد الإلكتروني:</label>
        <input type="email" name="email" class="form-control">
    </div>
    <div class="form-group">
        <label>نوع الرسالة:</label>
        <select class="form-control" name="Category" required="required">
            <option>نشر مقال</option>
            <option>إقتراح</option>
            <option>شكوى</option>
            <option>أخرى</option>
        </select>
    </div>
    <hr>
    <div class="form-group mt-3">
        <label>رسالتك:</label>
<br><textarea type="text" name="message" class="form-control" required="required" rows="7"></textarea>
    </div>
    <div class="form-group mt-3">
        <label class="mr-2">إرفاق ملف:</label><br>
        <input type="file" name="file">
    </div>
    <hr>
        <button type="submit" class="btn btn-secondary">إرسال</button>
    <p class="success">تم الإرسال.</p>
    <p class="fail">حصل خطأ بالإرسال، فضلًا حاول مرةً ثانية.</p>
</div>
</form>
<script src='http://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js'></script>
<script type="text/javascript">
$(".formID").submit(function(e){
  e.preventDefault();
  var action = $(this).attr("action");
  $.ajax({
    type: "POST",
    url: action,
    crossDomain: true,
    data: new FormData(this),
    dataType: "json",
    contentType: "multipart/form-data",
    processData: false,
    contentType: false,
    headers: {
      "Accept": "application/json"
    }
  }).done(function() {
     $(".success").addClass("is-active");
     $(".fail").removeClass("is-active");
  }).fail(function() {
     $(".fail").addClass("is-active");
     $(".success").removeClass("is-active");
  });
});
</script>
