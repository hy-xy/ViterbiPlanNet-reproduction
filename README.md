# ViterbiPlanNet 复现验证

对论文《ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Planning in Instructional Videos》（CVPR 2026）的复现验证。

- 基于原论文作者官方开源代码完成复现与验证，未对代码进行任何修改。
- 本仓库为个人复现记录，非原创工作。
- 原论文官方代码：https://github.com/Gigi-G/ViterbiPlanNet

## 复现结果

<table border="1" cellspacing="0" cellpadding="5" style="text-align: center; width: 100%; border-collapse: collapse;">
  <thead>
    <tr>
      <th rowspan="2">T</th>
      <th rowspan="2"></th>
      <th colspan="4">CrossTask</th>
      <th colspan="4">COIN</th>
      <th colspan="4">NIV</th>
    </tr>
    <tr>
      <th>SR(%)↑</th><th>mAcc(%)↑</th><th>mIoU(%)↑</th><th>Params(M)</th>
      <th>SR(%)↑</th><th>mAcc(%)↑</th><th>mIoU(%)↑</th><th>Params(M)</th>
      <th>SR(%)↑</th><th>mAcc(%)↑</th><th>mIoU(%)↑</th><th>Params(M)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">3</td>
      <td>复现</td>
      <td>38.76</td><td>63.28</td><td>84.03</td><td>5.55</td>
      <td>34.04</td><td>50.89</td><td>84.26</td><td>6.07</td>
      <td>32.22</td><td>47.16</td><td>74.59</td><td>5.48</td>
    </tr>
    <tr>
      <td>论文</td>
      <td>38.45</td><td>63.07</td><td>83.89</td><td>5.57</td>
      <td>33.99</td><td>50.87</td><td>83.88</td><td>6.67</td>
      <td>32.37</td><td>46.96</td><td>73.85</td><td>5.48</td>
    </tr>
    <tr>
      <td rowspan="2">4</td>
      <td>复现</td>
      <td>24.54</td><td>56.74</td><td>81.26</td><td>5.58</td>
      <td>23.86</td><td>45.43</td><td>82.29</td><td>6.27</td>
      <td>27.19</td><td>47.37</td><td>75.68</td><td>5.49</td>
    </tr>
    <tr>
      <td>论文</td>
      <td>24.64</td><td>57.00</td><td>81.18</td><td>5.6</td>
      <td>23.92</td><td>45.63</td><td>82.56</td><td>6.87</td>
      <td>27.54</td><td>45.55</td><td>74.71</td><td>5.50</td>
    </tr>
    <tr>
      <td rowspan="2">5</td>
      <td>复现</td>
      <td>16.14</td><td>53.38</td><td>79.58</td><td>5.62</td>
      <td>15.67</td><td>39.43</td><td>81.59</td><td>6.47</td>
      <td>22.99</td><td>42.14</td><td>73.90</td><td>5.51</td>
    </tr>
    <tr>
      <td>论文</td>
      <td>15.97</td><td>53.30</td><td>79.56</td><td>5.64</td>
      <td>15.87</td><td>39.42</td><td>81.19</td><td>7.07</td>
      <td>23.10</td><td>42.97</td><td>74.81</td><td>5.51</td>
    </tr>
    <tr>
      <td rowspan="2">6</td>
      <td>复现</td>
      <td>10.48</td><td>49.35</td><td>77.66</td><td>5.65</td>
      <td>12.68</td><td>35.74</td><td>78.49</td><td>6.67</td>
      <td>18.24</td><td>44.82</td><td>75.27</td><td>5.52</td>
    </tr>
    <tr>
      <td>论文</td>
      <td>10.37</td><td>49.25</td><td>78.01</td><td>5.67</td>
      <td>13.11</td><td>36.03</td><td>79.35</td><td>7.27</td>
      <td>18.78</td><td>45.77</td><td>75.91</td><td>5.52</td>
    </tr>
  </tbody>
</table>

## 说明
- 复现结果与论文报告值高度接近，验证了可微分 Viterbi 层与过程知识图谱端到端训练的有效性。
- 数据集与模型权重较大，未上传至仓库。
