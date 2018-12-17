# FacebookFanpage
## Add đoạn script này vào dưới thẻ mở của thẻ body:
```
<!-- Load Facebook SDK for JavaScript -->
<div id="fb-root"></div>
<script>
    window.fbAsyncInit = function () {
      FB.init({
        appId: '308419149774448',
        autoLogAppEvents: true,
        xfbml: true,
        version: 'v2.12'
      });
    };
    (function(d, s, id) {
    var js, fjs = d.getElementsByTagName(s)[0];
    if (d.getElementById(id)) return;
    js = d.createElement(s); js.id = id;
    js.src = 'https://connect.facebook.net/vi_VN/sdk/xfbml.customerchat.js';
    fjs.parentNode.insertBefore(js, fjs);
    }(document, 'script', 'facebook-jssdk'));
</script>
```

## Add đoạn script dưới đấy vào bất kỳ trang nào bạn muốn hiển thị chatbox, nếu muốn hiển thị ở tất cả các trang thì add vào trang index hoặc trang root
```
<!-- Your customer chat code -->
<div 
    class="fb-customerchat" 
    attribution=setup_tool 
    page_id="1412841702305858" 
    theme_color="#0084ff"
    logged_in_greeting="Xin chào, Puzzle Studio có thể giúp gì cho bạn?"
    logged_out_greeting="Xin chào, Puzzle Studio có thể giúp gì cho bạn?" 
    greeting_dialog_display="show">
</div>
```

* page_id: thay id của fanpage vào
* theme_color: đổi màu cho chatbox
* logged_in_greeting, logged_out_greeting: Lời chào đầu tiên

Sau khi add thì liên hệ chủ fanpage, yêu cầu họ vào phần fanpage settings -> Messengers Platform -> White-listed domains -> Add các domains mà bạn cho phép hiển thị. Ví dụ: teahouse.com, mamconcept.com
# Done
