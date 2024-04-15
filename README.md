# Toggle-off-responsive-with-js
Toggle off responisve with js
// // 		------toggle serves js---
var windowWidth = $(window).width(); // Get initial window width

    // Check window width on resize
    $(window).resize(function() {
        windowWidth = $(window).width();
    });

    $(".services-item").click(function() {
        // Check if window width is greater than 980px
        if (windowWidth > 980) {
            $(this).toggleClass("toggle-item");
            $(this).find(".services-toggle-content").slideToggle("slow");
            $(this).find(".services-toggle-title .et_pb_blurb_description").toggleClass('description');
            $(this).parent().toggleClass('services-item-row');
        }
    });


		
    }); 
