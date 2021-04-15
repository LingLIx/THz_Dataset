<!DOCTYPE html>
<!-- modified from url=(0049)https://github.com/shijieS/DMMN_Page -->
<html class="gr__ee_nthu_edu" lang="en">

<head>
  <meta content="text/html; charset=UTF-8" http-equiv="Content-Type">
  <meta content="IE=edge" http-equiv="X-UA-Compatible">
  <meta content="width=device-width, initial-scale=1" name="viewport">
  <meta content="XueFei" name="author">
  <title>An Active Terahertz Imaging Dataset for Concealed Multi-object Detection and Evaluation</title>

  <!-- CSS includes -->
  <link href="./asset/bootstrap.min.css" rel="stylesheet">
  <link href="./asset/css" rel="stylesheet" type="text/css">
  <link href="./asset/mystyle.css" rel="stylesheet">
</head>

<body data-gr-c-s-loaded="true">

<div class="topnav" id="myTopnav">
  <a href="#header">Home</a>
  <a href="#abstract">Abstract</a>
  <a href="#dataset">Dataset</a>
  <a href="#paper">Paper</a>
  <a href="#acknowledgement">Acknowledgements</a>
  <a class="icon" href="javascript:void(0);" onclick="toggleTopNav()">&#9776;</a>
</div>


<div class="container-fluid" id="header">
  <div class="row">
    <h1>An Active Terahertz Imaging Dataset for Concealed Multi-object Detection and Evaluation</h1>
    <div class="authors">

      <a href="https://scholar.google.com/citations?user=oKE2Wx8AAAAJ&hl=en&oi=ao" target="_blank">Dong Liang,</a>
      Fei Xue
      <br><br>

      <p style="text-align:center;">
        <a href="https://www.nuaa.edu.cn/" target="_blank">
          <img height="100" src="./ICASSP2021/nuaa.jpg">
        </a>
        <a href="http://cs.nuaa.edu.cn/" target="_blank">
          <img height="100" src="./ICASSP2021/nuaa-ccst.png">
        </a>
        <a href="http://cs.nuaa.edu.cn/" target="_blank">
          <img height="100" src="./ICASSP2021/nuaa-ai.png">
        </a>
        <a href="https://soft2011.nju.edu.cn/" target="_blank">
          <img height="100" src="./ICASSP2021/cicnsti.png">
        </a>
      </p>

    </div>
  </div>
</div>


<div class="container" id="abstract">
  <h2>Abstract</h2>
  <p style="text-align:justify;">
    Concealed objects detection in Terahertz imaging is an urgent need for public security and counter-terrorism.
    So far, there is no public Terahertz imaging dataset for evaluation of objects detection algorithms. This paper
    provides a public dataset for evaluating multi-object detection algorithms in active Terahertz imaging worked at
    140 GHz, with the imaging resolution 5 mm by 5 mm. Due to poor imaging quality, object detection on this dataset
    is much more difficult than on those commonly used public object detection datasets in computer vision field.
    Several state-of-the-art computer vision based detectors, including YOLOv3, YOLOv4, FRCN-OHEM and RetinaNet, are
    evaluated on this dataset. In addition, we enhance RetinaNet through embedding low-level features for detecting
    small objects. Aiming at solving the problem of unbalanced and hard training samples, Focal Loss and Online Hard
    Example Mining technology are discussed and employed. Experimental results show that the enhanced RetinaNet
    achieves the best mAP with fast detection speed which can meet the requirement of real-time security inspection.
    Experiment also indicates that hiding objects in different parts of the human body affect the detection accuracy.
  </p>
</div>


<div class="container" id="dataset">
  <h2>Dataset</h2>

  <p style="text-align:center;">
    <img width="100%" src="./ICASSP2021/classes.png">
    <br>Sample display for each category. The bottom row shows a zoomed-in view of the object.
  </p><br><br>

  <p style="text-align:center;">
    <img width="100%" src="./ICASSP2021/diversification.png">
    <br>Sample display for diversification.
  </p>
  <br>

  <h3>Dataset information:</h3>
    Category table:<br>
    <table style="width:100%;" border=1>
      <tr>
        <th>Class</th>
        <td>GA</td>
        <td>KK</td>
        <td>SS</td>
        <td>MD</td>
        <td>CK</td>
        <td>WB</td>
        <td>KC</td>
        <td>CP</td>
        <td>CL</td>
        <td>LW</td>
        <td>UN</td>
      </tr>
      <tr>
        <th>Item</th>
        <td>Gun</td>
        <td>Kitchen Knife</td>
        <td>Scissors</td>
        <td>Metal Dagger</td>
        <td>Ceramic Knife</td>
        <td>Water Bottle</td>
        <td>Key Chain</td>
        <td>Cell Phone</td>
        <td>Cigarette Lighter</td>
        <td>Leather Wallet</td>
        <td>Unknown</td>
      </tr>
      <tr>
        <th>Quantity</th>
        <td>116</td>
        <td>100</td>
        <td>96</td>
        <td>64</td>
        <td>129</td>
        <td>107</td>
        <td>78</td>
        <td>129</td>
        <td>163</td>
        <td>78</td>
        <td>289</td>
      </tr>
    </table>
    <br>
    Dataset format table:
    <table style="width:100%;" border=1>
      <tr>
        <th>Number of images</th>
        <th>Image size and format</th>
        <th>Imaging resolution</th>
        <th>Models</th>
        <th>Number of categories</th>
        <th>Objects per image</th>
        <th>Maximum object size</th>
        <th>Average object size</th>
        <th>Minimum object size</th>
      </tr>
      <tr>
        <td>3157</td>
        <td>335×880 p.x. JPEG</td>
        <td>5×5 mm</td>
        <td>4 males, 6 females</td>
        <td>11</td>
        <td>0,1,2,3</td>
        <td>13390 p.x.</td>
        <td>3222 p.x.</td>
        <td>390 p.x.</td>
      </tr>
    </table>

  <h3>Dataset structure:</h3>
    THZ_dataset_det_VOC<br>
    &emsp;&emsp;├── Annotations<br>
    &emsp;&emsp;│ &emsp;&emsp; ├── D_N_F1_CK_F_LA_WB_F_S_back_0907140917.xml<br>
    &emsp;&emsp;│ &emsp;&emsp; ├── D_N_F1_CK_F_LA_WB_F_S_front_0907140917.xml<br>
    &emsp;&emsp;│ &emsp;&emsp; ├── D_N_F1_CL_V_LA_LW_V_RA_back_0907141138.xml<br>
    &emsp;&emsp;│ &emsp;&emsp; ├── ...<br>
    &emsp;&emsp;│ &emsp;&emsp; └── T_P_M6_MD_F_LL_CK_F_C_WB_F_RT_front_0906154134.xml<br>
    &emsp;&emsp;└── JPEGImages<br>
    &emsp;&emsp;&emsp;&emsp;&emsp; ├── D_N_F1_CK_F_LA_WB_F_S_back_0907140917.jpg<br>
    &emsp;&emsp;&emsp;&emsp;&emsp; ├── D_N_F1_CK_F_LA_WB_F_S_front_0907140917.jpg<br>
    &emsp;&emsp;&emsp;&emsp;&emsp; ├── D_N_F1_CL_V_LA_LW_V_RA_back_0907141138.jpg<br>
    &emsp;&emsp;&emsp;&emsp;&emsp; ├── ...<br>
    &emsp;&emsp;&emsp;&emsp;&emsp; └── T_P_M6_MD_F_LL_CK_F_C_WB_F_RT_front_0906154134.jpg<br>
    <br>
    THZ_dataset_seg_IMG<br>
    &emsp;&emsp;├── train<br>
    &emsp;&emsp;├── val<br>
    &emsp;&emsp;└── test<br>
    <br>


  <h3>Download links:</h3>
  <div class="row">
    <div class="col-md-4">
      <a href="https://drive.google.com/drive/folders/1A6LiyWAvRmKIJN5yXQZ3HxZVwNEFz8uV?usp=sharing" target="_blank">
        <p style="text-align:center;">
          <img width="100" src="./ICASSP2021/google-cloud.jpg"><br>
          Google drive<br>
      </a>
    </div>

    <div class="col-md-4">
      <a href="https://pan.baidu.com/s/1MRPyeMtzCQRO5ydgX0rSHA" target="_blank">
        <p style="text-align:center;">
          <img width="100" src="./ICASSP2021/baidu-cloud.jpg"><br>
          Baidu drive<br>
      </a>
      (Extraction code: x3od)
    </div>

    <div class="col-md-4">
      <a href="https://pan.nuaa.edu.cn/share/5cb047f309049ba7f68ab9e1e0" target="_blank">
        <p style="text-align:center;">
          <img width="100" src="./ICASSP2021/nuaa.jpg"><br>
          NUAA drive<br>
      </a>
    </div>

  </div>

</div>


<div class="container" id="paper">
  <h2>Todo</h2>
<!--
  <div>
    <pre class="citation">@inproceedings{DLiang2021,
    author = {Dong Liang, Fei Xue},
    title = {An Active Terahertz Imaging Dataset for Concealed Multi-object Detection and Evaluation},
    booktitle = {International Conference on Acoustics, Speech and Signal Processing (ICASSP2021)},
    year = {2021}
}</pre>
  </div>
-->
</div>


<div class="container" id="acknowledgement">
  <h2>Acknowledgements</h2>
  <p style="text-align:center;">
    <a href="https://www.nuaa.edu.cn/" target="_blank">
      <img height="100" src="./ICASSP2021/nuaa.jpg">
    </a>
    <a href="http://cs.nuaa.edu.cn/" target="_blank">
      <img height="100" src="./ICASSP2021/nuaa-ccst.png">
    </a>
    <a href="http://cs.nuaa.edu.cn/" target="_blank">
      <img height="100" src="./ICASSP2021/nuaa-ai.png">
    </a>
    <a href="https://soft2011.nju.edu.cn/" target="_blank">
      <img height="100" src="./ICASSP2021/cicnsti.png">
    </a>
    <a href="https://www.caep.cn/" target="_blank">
      <img height="100" src="./ICASSP2021/caep.jpg">
    </a>
    <a href="https://www.nvidia.com" target="_blank">
      <img height="100" src="./ICASSP2021/nvidia.jpg">
    </a>
    <a href="https://www.tensorflow.org/" target="_blank">
      <img height="100" src="./ICASSP2021/tensorflow.png">
    </a>
  </p>
</div>


<div id="footer">
  <br>
  <p style="text-align:center;">
    Copyright © Fei Xue 2021 Based on
    <a href="https://github.com/shijieS/DMMN_Page" target="_blank">DMMN</a>
    <br>Last modified on January 13, 2021
  </p>
</div>


<!-- Javascript includes -->
<script src="./asset/jquery-1.8.3.min.js"></script>
<script src="./asset/mystyle.js"></script>
<script src="./asset/bootstrap.min.js"></script>
<script async="" src="./asset/analytics.js"></script>
<script>
  (function (i, s, o, g, r, a, m) {
      i['GoogleAnalyticsObject'] = r;
      i[r] = i[r] || function () {
          (i[r].q = i[r].q || []).push(arguments)
      }, i[r].l = 1 * new Date();
      a = s.createElement(o),
          m = s.getElementsByTagName(o)[0];
      a.async = 1;
      a.src = g;
      m.parentNode.insertBefore(a, m)
  })(window, document, 'script', '//www.google-analytics.com/analytics.js', 'ga');
  ga('create', 'UA-98479202-1', 'auto');
  ga('send', 'pageview');
</script>

<div id="point-jawn" style="z-index: 2147483647;"></div>
</body>
</html>
