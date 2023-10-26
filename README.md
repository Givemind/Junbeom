
<!DOCTYPE html>
<html>

<head>

  <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>

  <script type="text/javascript">
    google.charts.load("current", { packages: ["timeline"] });
    google.charts.setOnLoadCallback(drawChart);
    function drawChart() {

      var container = document.getElementById('example3.1');
      var chart = new google.visualization.Timeline(container);
      var dataTable = new google.visualization.DataTable();
      dataTable.addColumn({ type: 'string', id: 'Position' });
      dataTable.addColumn({ type: 'string', id: 'Name' });
      dataTable.addColumn({ type: 'date', id: 'Start' });
      dataTable.addColumn({ type: 'date', id: 'End' });
      dataTable.addRows([
        ['1대 태조', '태조', new Date(1335, 2, 4), new Date(1392, 2, 4)],
        ['1대 태조', '재위', new Date(1392, 2, 4), new Date(1398, 2, 4),],
        ['2대 정종', '정종', new Date(1357, 2, 4), new Date(1398, 2, 4)],
        ['2대 정종', '재위', new Date(1398, 2, 4), new Date(1400, 2, 4)],
        ['3대 태종', '태종', new Date(1367, 1, 1), new Date(1400, 2, 3)],
        ['3대 태종', '재위', new Date(1400, 2, 4), new Date(1418, 2, 4)],
        ['4대 세종', '세종', new Date(1397, 2, 4), new Date(1418, 2, 4)],
        ['4대 세종', '재위', new Date(1418, 2, 4), new Date(1450, 2, 4)],
        ['5대 문종', '문종', new Date(1414, 2, 4), new Date(1450, 2, 4)],
        ['5대 문종', '재위', new Date(1450, 2, 4), new Date(1452, 2, 4)],
        ['6대 단종', '단종', new Date(1441, 2, 4), new Date(1452, 2, 4)],
        ['6대 단종', '재위', new Date(1452, 2, 4), new Date(1455, 2, 4)],
        ['7대 세조', '세조', new Date(1417, 2, 4), new Date(1455, 2, 4)],
        ['7대 세조', '재위', new Date(1455, 2, 4), new Date(1468, 2, 4)],
        ['8대 예종', '에종', new Date(1450, 2, 4), new Date(1468, 2, 4)],
        ['8대 예종', '재위', new Date(1468, 2, 4), new Date(1469, 2, 4)],
        ['9대 성종', '성종', new Date(1457, 2, 4), new Date(1469, 2, 4)],
        ['9대 성종', '재위', new Date(1469, 2, 4), new Date(1494, 2, 4)],
        ['10대 연산군', '연산군', new Date(1476, 2, 4), new Date(1494, 2, 4)],
        ['10대 연산군', '재위', new Date(1494, 2, 4), new Date(1506, 2, 4)],
        ['11대 중종', '중종', new Date(1488, 2, 4), new Date(1506, 2, 4)],
        ['11대 중종', '재위', new Date(1506, 2, 4), new Date(1544, 2, 4)],
        ['12대 인종', '인종', new Date(1515, 2, 4), new Date(1544, 2, 4)],
        ['12대 인종', '재위', new Date(1544, 2, 4), new Date(1545, 2, 4)],
        ['13대 명종', '명종', new Date(1534, 2, 4), new Date(1545, 2, 4)],
        ['13대 명종', '재위', new Date(1545, 2, 4), new Date(1567, 2, 4)],
        ['14대 선조', '선조', new Date(1552, 2, 4), new Date(1567, 2, 4)],
        ['14대 선조', '재위', new Date(1567, 2, 4), new Date(1608, 2, 4)],
        ['15대 광해군', '광해군', new Date(1575, 2, 4), new Date(1608, 2, 4)],
        ['15대 광해군', '재위', new Date(1608, 2, 4), new Date(1623, 2, 4)],
        ['16대 인조', '인조', new Date(1595, 2, 4), new Date(1623, 2, 4)],
        ['16대 인조', '재위', new Date(1623, 2, 4), new Date(1649, 2, 4)],
        ['17대 효종', '효종', new Date(1619, 2, 4), new Date(1649, 2, 4)],
        ['17대 효종', '재위', new Date(1649, 2, 4), new Date(1659, 2, 4)],
        ['18대 현종', '현종', new Date(1641, 2, 4), new Date(1659, 2, 4)],
        ['18대 현종', '재위', new Date(1659, 2, 4), new Date(1674, 2, 4)],
        ['19대 숙종', '숙종', new Date(1661, 2, 4), new Date(1674, 2, 4)],
        ['19대 숙종', '재위', new Date(1674, 2, 4), new Date(1720, 2, 4)],
        ['20대 경종', '경종', new Date(1688, 2, 4), new Date(1720, 2, 4)],
        ['20대 경종', '재위', new Date(1720, 2, 4), new Date(1724, 2, 4)],
        ['21대 영조', '영조', new Date(1694, 2, 4), new Date(1724, 2, 4)],
        ['21대 영조', '재위', new Date(1724, 2, 4), new Date(1776, 2, 4)],
        ['22대 정조', '정조', new Date(1752, 2, 4), new Date(1776, 2, 4)],
        ['22대 정조', '재위', new Date(1776, 2, 4), new Date(1800, 2, 4)],
        ['23대 순조', '순조', new Date(1790, 2, 4), new Date(1800, 2, 4)],
        ['23대 순조', '재위', new Date(1800, 2, 4), new Date(1834, 2, 4)],
        ['24대 헌종', '현종', new Date(1827, 2, 4), new Date(1834, 2, 4)],
        ['24대 헌종', '재위', new Date(1834, 2, 4), new Date(1849, 2, 4)],
        ['25대 철종', '철종', new Date(1831, 2, 4), new Date(1849, 2, 4)],
        ['25대 철종', '재위', new Date(1849, 2, 4), new Date(1863, 2, 4)],
        ['26대 고종', '고종', new Date(1852, 2, 4), new Date(1863, 2, 4)],
        ['26대 고종', '재위', new Date(1863, 2, 4), new Date(1897, 2, 4)],
        ['대한제국 1대 고종', '고종', new Date(1852, 2, 4), new Date(1897, 2, 4)],
        ['대한제국 2대 순종', '순종', new Date(1874, 2, 4), new Date(1907, 2, 4)],]);

      var options = {
        colors: ['#123456', 'rgb(66, 133, 244)'],
      };

      chart.draw(dataTable, options);
    }
  </script>

<body>


  <div id="example3.1" style="height: 100%;"></div>
</body>

</head>

</html>
