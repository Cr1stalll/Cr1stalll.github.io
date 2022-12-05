<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>index</title>
    <!-- 定义样式 -->
    <style>
        .middle{
            width: 800px;
            height: 500px;
            margin-left: 20%;
        }
        .clock{
            margin-left: 85%;
        }
        h1{
            text-align: center;
            font-style: italic;
        }
        table{
            border-collapse: collapse;
            border: 1px solid;
            border-color: rgb(185, 189, 193);
            text-align: center;
            width: 400px;
            height: 30px;
        }
        td{
            border-collapse: collapse;
            border: 1px solid;
            border-color: rgb(185, 189, 193);
            text-align: center;
            width: 300px;
            height: 30px;
            background-color: rgb(223, 217, 217);
        }
        th{
            border-collapse: collapse;
            border: 1px solid;
            border-color: rgb(185, 189, 193);
            text-align: center;
            width: 300px;
            height: 30px;
        }
    </style>
</head>
<body>
    <!-- 定义函数 -->
    <script type="text/javascript">
        function getDate(){
            var d = new Date();
            var year = d.getFullYear();
            var month = d.getMonth()+1;
            var date = d.getDate();
                //document.write(year+"年"+month+"月"+date+"日"); 
                return year+"年"+month+"月"+date+"日"
            }
        function getTime(){
            var t=new Date();
            var hour=t.getHours();
            var minutie=t.getMinutes();
            var second=t.getSeconds();
                //document.write(hour+"时" +minutie+"分" +second+"秒") 
                return hour+"时" +minutie+"分" +second+"秒"
            }

        function showDate(){
            document.querySelector(".clock").innerText = getDate()+getTime()
        }
        setInterval(() => {
            showDate()
        }, 1000);

    </script>
    <div class="clock"></div>
    <div class="middle">
        <h1>Welcome to my website</h1>
        <h2>Experiment1</h2>
        <table>
            <thead>
                <tr>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>EXP-a</td>
                    <td>EXP-b</td>
                    <td>EXP-c</td>
                    <td>EXP-d</td>
                </tr>
            </tbody>
        </table>
        <br>
        <h2>Experiment2</h2>
        <table>
            <thead>
                <tr>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>EXP</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
            </tbody>
        </table>
        <br>
        <h2>Experiment3</h2>
        <table>
            <thead>
                <tr>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                    <th> </th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>EXP-a</td>
                    <td>EXP-b</td>
                    <td>EXP-c</td>
                    <td>EXP-d</td>
                </tr>
                <tr>
                    <td>EXP-e</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
            </tbody>
        </table>
    </div>
</body>
</html>
