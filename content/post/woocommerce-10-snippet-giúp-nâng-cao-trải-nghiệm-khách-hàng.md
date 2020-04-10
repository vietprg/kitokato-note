+++
author = "viet.m"
cover = ""
date = 2020-04-09T22:00:00Z
description = "Có nhiều cách đơn giản để bạn nâng cao khả năng bán hàng cùng với WooCommerce mà không cần phải dùng những plugins khiến trang web thêm nặng nề."
tags = ["woocommerce tips", " woocommerce snippets"]
title = "WooCommerce: 10 snippet giúp nâng cao trải nghiệm khách hàng"

+++
Bài viết đầu tiên này xin chia sẻ cùng các bạn 10 snippet tuyệt vời nhất, giúp trải nghiệm bán hàng của bạn trở nên tuyệt vời hơn trong mắt khách hàng.

**Điều đặc biệt là bạn không cần phải cài thêm bất kỳ plugins hỗ trợ nào cả.**

Hãy bắt đầu với:

1. Thêm ghi chú đặc biệt dưới tên của sản phẩm. Ví dụ như: "Hãy gửi đơn hàng trước 12:00 để nhận hàng ngay hôm nay".

       /**
        * @snippet       Thêm ghi chú đặc biệt trên trang sản phẩm
        * @how-to        Custom WooCommerce
        * @sourcecode    https://viet.md
        * @author        viet.m
        * @compatible    WooCommerce 3.5.4
        */
        
       add_action( 'woocommerce_single_product_summary', 'bbloomer_display_pressure_badge', 6 );
          
       function bbloomer_display_pressure_badge() {
           echo '<div class="woocommerce-message">Order by 6pm and get it delivered tomorrow!</div>';
       }

![](/uploads/pressure.png)