$.ajax({
                type: "POST",
                url: "http://localhost:50526/DataService.asmx/HelloWorld",
                data: "{}",
                contentType: "application/json; charset=utf-8",
                dataType: "json",
                success: function (msg) {
                    $("#output").text(msg.d);
                },
                error: function (err) {
                    alert(err);
                }
});

$.ajax({
                    type: "POST",
                    url: "http://localhost:50526/DataService.asmx/CheckUser",
                    data: "{userid: 'a', password: 'b'}",
                    contentType: "application/json; charset=utf-8",
                    dataType: "json",
                    success: function (msg) {
                        $("#output").text(msg.d);
                    },
                    error: function (err) {
                        alert(err);
                    }
});
