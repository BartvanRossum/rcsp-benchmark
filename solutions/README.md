# Solution File Format

Solutions are split into two subfolders, one per instance variant (see the top-level [README](../README.md)):
- `single_depot/solution_single_depot_s{S}_t{T}.txt`
- `multi_depot/solution_multi_depot_s{S}_t{T}.txt`

Each solution file contains one duty per line.
Each line is a space-separated list of connection indices, corresponding to a valid duty in the instance `s{S}_t{T}`.

A duty is a path SOURCE → CONNECTION* → SINK in the connection graph, where the SOURCE and SINK connections use the same depot station. The connection indices refer to the `index` field in `connections_single_depot.txt` (for `single_depot/` solutions) or `connections_multi_depot.txt` (for `multi_depot/` solutions).

These are the best known solutions found throughout the experiments in the accompanying paper.

## Best Known Solutions

<table>
<thead>
<tr>
<th rowspan="2">Instance</th>
<th colspan="5">Single-depot</th>
<th colspan="5">Multi-depot</th>
</tr>
<tr>
<th>Root LB</th>
<th>Best LB</th>
<th>Best UB</th>
<th>Gap (%)</th>
<th>Duties</th>
<th>Root LB</th>
<th>Best LB</th>
<th>Best UB</th>
<th>Gap (%)</th>
<th>Duties</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>s2_t90</code></td>
<td align="right">745,680</td>
<td align="right">748,080</td>
<td align="right">748,080</td>
<td align="right">0</td>
<td align="right">14</td>
<td align="right">728,800</td>
<td align="right">748,080</td>
<td align="right">748,080</td>
<td align="right">0</td>
<td align="right">14</td>
</tr>
<tr>
<td><code>s2_t118</code></td>
<td align="right">1,212,642</td>
<td align="right">1,221,780</td>
<td align="right">1,221,780</td>
<td align="right">0</td>
<td align="right">22</td>
<td align="right">1,200,240</td>
<td align="right">1,201,140</td>
<td align="right">1,201,140</td>
<td align="right">0</td>
<td align="right">21</td>
</tr>
<tr>
<td><code>s2_t120</code></td>
<td align="right">997,710</td>
<td align="right">1,010,640</td>
<td align="right">1,010,640</td>
<td align="right">0</td>
<td align="right">19</td>
<td align="right">975,560</td>
<td align="right">983,880</td>
<td align="right">983,880</td>
<td align="right">0</td>
<td align="right">18</td>
</tr>
<tr>
<td><code>s2_t122</code></td>
<td align="right">719,000</td>
<td align="right">740,280</td>
<td align="right">740,280</td>
<td align="right">0</td>
<td align="right">14</td>
<td align="right">711,060</td>
<td align="right">716,460</td>
<td align="right">716,460</td>
<td align="right">0</td>
<td align="right">13</td>
</tr>
<tr>
<td><code>s2_t131</code></td>
<td align="right">1,139,400</td>
<td align="right">1,147,500</td>
<td align="right">1,147,500</td>
<td align="right">0</td>
<td align="right">21</td>
<td align="right">1,123,140</td>
<td align="right">1,123,920</td>
<td align="right">1,123,920</td>
<td align="right">0</td>
<td align="right">20</td>
</tr>
<tr>
<td><code>s3_t168</code></td>
<td align="right">1,441,980</td>
<td align="right">1,441,980</td>
<td align="right">1,441,980</td>
<td align="right">0</td>
<td align="right">26</td>
<td align="right">1,411,155</td>
<td align="right">1,414,680</td>
<td align="right">1,414,680</td>
<td align="right">0</td>
<td align="right">26</td>
</tr>
<tr>
<td><code>s3_t172</code></td>
<td align="right">1,211,690</td>
<td align="right">1,228,380</td>
<td align="right">1,228,380</td>
<td align="right">0</td>
<td align="right">22</td>
<td align="right">1,199,043</td>
<td align="right">1,209,480</td>
<td align="right">1,209,480</td>
<td align="right">0</td>
<td align="right">21</td>
</tr>
<tr>
<td><code>s3_t228</code></td>
<td align="right">1,849,665</td>
<td align="right">1,855,440</td>
<td align="right">1,855,440</td>
<td align="right">0</td>
<td align="right">33</td>
<td align="right">1,811,664</td>
<td align="right">1,819,200</td>
<td align="right">1,819,200</td>
<td align="right">0</td>
<td align="right">33</td>
</tr>
<tr>
<td><code>s3_t232</code></td>
<td align="right">1,568,227</td>
<td align="right">1,575,840</td>
<td align="right">1,575,840</td>
<td align="right">0</td>
<td align="right">27</td>
<td align="right">1,558,232</td>
<td align="right">1,561,560</td>
<td align="right">1,561,560</td>
<td align="right">0</td>
<td align="right">27</td>
</tr>
<tr>
<td><code>s3_t262</code></td>
<td align="right">1,850,628</td>
<td align="right">1,862,520</td>
<td align="right">1,862,520</td>
<td align="right">0</td>
<td align="right">32</td>
<td align="right">1,749,558</td>
<td align="right">1,761,300</td>
<td align="right">1,761,300</td>
<td align="right">0</td>
<td align="right">31</td>
</tr>
<tr>
<td><code>s3_t300</code></td>
<td align="right">1,992,091</td>
<td align="right">2,005,200</td>
<td align="right">2,005,200</td>
<td align="right">0</td>
<td align="right">36</td>
<td align="right">1,939,398</td>
<td align="right">1,941,660</td>
<td align="right">1,941,660</td>
<td align="right">0</td>
<td align="right">35</td>
</tr>
<tr>
<td><code>s3_t337</code></td>
<td align="right">2,542,520</td>
<td align="right">2,552,400</td>
<td align="right">2,552,400</td>
<td align="right">0</td>
<td align="right">43</td>
<td align="right">2,375,106</td>
<td align="right">2,383,200</td>
<td align="right">2,383,200</td>
<td align="right">0</td>
<td align="right">41</td>
</tr>
<tr>
<td><code>s4_t273</code></td>
<td align="right">1,161,816</td>
<td align="right">1,169,640</td>
<td align="right">1,169,640</td>
<td align="right">0</td>
<td align="right">21</td>
<td align="right">1,117,997</td>
<td align="right">1,118,460</td>
<td align="right">1,118,460</td>
<td align="right">0</td>
<td align="right">20</td>
</tr>
<tr>
<td><code>s4_t290</code></td>
<td align="right">1,671,952</td>
<td align="right">1,676,820</td>
<td align="right">1,676,820</td>
<td align="right">0</td>
<td align="right">30</td>
<td align="right">1,631,119</td>
<td align="right">1,633,680</td>
<td align="right">1,633,680</td>
<td align="right">0</td>
<td align="right">29</td>
</tr>
<tr>
<td><code>s4_t297</code></td>
<td align="right">1,711,780</td>
<td align="right">1,725,720</td>
<td align="right">1,725,720</td>
<td align="right">0</td>
<td align="right">31</td>
<td align="right">1,660,696</td>
<td align="right">1,661,280</td>
<td align="right">1,661,280</td>
<td align="right">0</td>
<td align="right">30</td>
</tr>
<tr>
<td><code>s4_t311</code></td>
<td align="right">2,270,068</td>
<td align="right">2,272,440</td>
<td align="right">2,272,440</td>
<td align="right">0</td>
<td align="right">40</td>
<td align="right">2,205,150</td>
<td align="right">2,208,360</td>
<td align="right">2,208,360</td>
<td align="right">0</td>
<td align="right">40</td>
</tr>
<tr>
<td><code>s4_t313</code></td>
<td align="right">2,086,800</td>
<td align="right">2,095,620</td>
<td align="right">2,095,620</td>
<td align="right">0</td>
<td align="right">37</td>
<td align="right">1,994,272</td>
<td align="right">1,996,980</td>
<td align="right">1,996,980</td>
<td align="right">0</td>
<td align="right">35</td>
</tr>
<tr>
<td><code>s4_t320</code></td>
<td align="right">2,377,312</td>
<td align="right">2,385,300</td>
<td align="right">2,385,300</td>
<td align="right">0</td>
<td align="right">42</td>
<td align="right">2,313,277</td>
<td align="right">2,317,440</td>
<td align="right">2,317,440</td>
<td align="right">0</td>
<td align="right">41</td>
</tr>
<tr>
<td><code>s5_t333</code></td>
<td align="right">1,659,480</td>
<td align="right">1,659,480</td>
<td align="right">1,659,480</td>
<td align="right">0</td>
<td align="right">30</td>
<td align="right">1,584,592</td>
<td align="right">1,584,840</td>
<td align="right">1,584,840</td>
<td align="right">0</td>
<td align="right">30</td>
</tr>
<tr>
<td><code>s5_t349</code></td>
<td align="right">1,325,476</td>
<td align="right">1,333,560</td>
<td align="right">1,333,560</td>
<td align="right">0</td>
<td align="right">24</td>
<td align="right">1,250,717</td>
<td align="right">1,258,080</td>
<td align="right">1,258,080</td>
<td align="right">0</td>
<td align="right">22</td>
</tr>
<tr>
<td><code>s5_t385</code></td>
<td align="right">1,642,921</td>
<td align="right">1,651,380</td>
<td align="right">1,653,120</td>
<td align="right">0.11</td>
<td align="right">29</td>
<td align="right">1,570,116</td>
<td align="right">1,571,880</td>
<td align="right">1,571,880</td>
<td align="right">0</td>
<td align="right">28</td>
</tr>
<tr>
<td><code>s5_t409</code></td>
<td align="right">1,853,776</td>
<td align="right">1,854,900</td>
<td align="right">1,854,900</td>
<td align="right">0</td>
<td align="right">34</td>
<td align="right">1,813,958</td>
<td align="right">1,814,700</td>
<td align="right">1,814,700</td>
<td align="right">0</td>
<td align="right">34</td>
</tr>
<tr>
<td><code>s5_t413</code></td>
<td align="right">1,683,662</td>
<td align="right">1,701,840</td>
<td align="right">1,701,840</td>
<td align="right">0</td>
<td align="right">30</td>
<td align="right">1,623,060</td>
<td align="right">1,624,620</td>
<td align="right">1,624,620</td>
<td align="right">0</td>
<td align="right">29</td>
</tr>
<tr>
<td><code>s6_t450</code></td>
<td align="right">2,444,367</td>
<td align="right">2,451,720</td>
<td align="right">2,451,720</td>
<td align="right">0</td>
<td align="right">43</td>
<td align="right">2,363,507</td>
<td align="right">2,368,593</td>
<td align="right">2,370,540</td>
<td align="right">0.08</td>
<td align="right">42</td>
</tr>
<tr>
<td><code>s6_t482</code></td>
<td align="right">2,861,635</td>
<td align="right">2,864,880</td>
<td align="right">2,868,240</td>
<td align="right">0.12</td>
<td align="right">50</td>
<td align="right">2,688,349</td>
<td align="right">2,691,240</td>
<td align="right">2,691,240</td>
<td align="right">0</td>
<td align="right">49</td>
</tr>
<tr>
<td><code>s5_t501</code></td>
<td align="right">1,931,348</td>
<td align="right">1,942,468</td>
<td align="right">1,951,260</td>
<td align="right">0.45</td>
<td align="right">34</td>
<td align="right">1,871,901</td>
<td align="right">1,878,394</td>
<td align="right">1,879,800</td>
<td align="right">0.07</td>
<td align="right">33</td>
</tr>
<tr>
<td><code>s5_t591</code></td>
<td align="right">2,439,440</td>
<td align="right">2,440,976</td>
<td align="right">2,441,040</td>
<td align="right">0.00</td>
<td align="right">44</td>
<td align="right">2,341,780</td>
<td align="right">2,343,393</td>
<td align="right">2,346,600</td>
<td align="right">0.14</td>
<td align="right">42</td>
</tr>
<tr>
<td><code>s6_t514</code></td>
<td align="right">3,514,748</td>
<td align="right">3,528,422</td>
<td align="right">3,532,800</td>
<td align="right">0.12</td>
<td align="right">61</td>
<td align="right">3,196,426</td>
<td align="right">3,200,895</td>
<td align="right">3,202,320</td>
<td align="right">0.04</td>
<td align="right">57</td>
</tr>
<tr>
<td><code>s6_t518</code></td>
<td align="right">2,708,987</td>
<td align="right">2,712,000</td>
<td align="right">2,712,000</td>
<td align="right">0</td>
<td align="right">46</td>
<td align="right">2,558,366</td>
<td align="right">2,559,996</td>
<td align="right">2,560,920</td>
<td align="right">0.04</td>
<td align="right">46</td>
</tr>
<tr>
<td><code>s6_t521</code></td>
<td align="right">2,857,952</td>
<td align="right">2,869,128</td>
<td align="right">2,880,120</td>
<td align="right">0.38</td>
<td align="right">50</td>
<td align="right">2,690,373</td>
<td align="right">2,695,216</td>
<td align="right">2,696,580</td>
<td align="right">0.05</td>
<td align="right">48</td>
</tr>
<tr>
<td><code>s6_t580</code></td>
<td align="right">4,521,585</td>
<td align="right">4,534,807</td>
<td align="right">4,561,380</td>
<td align="right">0.58</td>
<td align="right">78</td>
<td align="right">4,312,151</td>
<td align="right">4,320,132</td>
<td align="right">4,330,920</td>
<td align="right">0.25</td>
<td align="right">76</td>
</tr>
<tr>
<td><code>s7_t570</code></td>
<td align="right">3,572,503</td>
<td align="right">3,588,419</td>
<td align="right">3,589,680</td>
<td align="right">0.04</td>
<td align="right">63</td>
<td align="right">3,375,250</td>
<td align="right">3,385,253</td>
<td align="right">3,391,680</td>
<td align="right">0.19</td>
<td align="right">60</td>
</tr>
<tr>
<td><code>s7_t599</code></td>
<td align="right">3,473,001</td>
<td align="right">3,482,597</td>
<td align="right">3,482,820</td>
<td align="right">0.01</td>
<td align="right">61</td>
<td align="right">3,280,091</td>
<td align="right">3,284,272</td>
<td align="right">3,297,480</td>
<td align="right">0.40</td>
<td align="right">58</td>
</tr>
<tr>
<td><code>s7_t627</code></td>
<td align="right">3,785,095</td>
<td align="right">3,796,950</td>
<td align="right">3,799,800</td>
<td align="right">0.08</td>
<td align="right">67</td>
<td align="right">3,536,373</td>
<td align="right">3,540,021</td>
<td align="right">3,545,940</td>
<td align="right">0.17</td>
<td align="right">63</td>
</tr>
<tr>
<td><code>s7_t681</code></td>
<td align="right">3,315,261</td>
<td align="right">3,333,440</td>
<td align="right">3,358,680</td>
<td align="right">0.75</td>
<td align="right">58</td>
<td align="right">3,084,196</td>
<td align="right">3,087,013</td>
<td align="right">3,096,240</td>
<td align="right">0.30</td>
<td align="right">55</td>
</tr>
<tr>
<td><code>s7_t695</code></td>
<td align="right">3,867,536</td>
<td align="right">3,873,529</td>
<td align="right">3,885,720</td>
<td align="right">0.31</td>
<td align="right">67</td>
<td align="right">3,619,377</td>
<td align="right">3,622,008</td>
<td align="right">3,625,620</td>
<td align="right">0.10</td>
<td align="right">65</td>
</tr>
<tr>
<td><code>s7_t738</code></td>
<td align="right">3,958,744</td>
<td align="right">3,968,197</td>
<td align="right">3,985,920</td>
<td align="right">0.44</td>
<td align="right">68</td>
<td align="right">3,657,380</td>
<td align="right">3,661,081</td>
<td align="right">3,668,820</td>
<td align="right">0.21</td>
<td align="right">65</td>
</tr>
<tr>
<td><code>s8_t628</code></td>
<td align="right">4,120,124</td>
<td align="right">4,129,320</td>
<td align="right">4,173,900</td>
<td align="right">1.07</td>
<td align="right">72</td>
<td align="right">3,736,804</td>
<td align="right">3,739,828</td>
<td align="right">3,746,820</td>
<td align="right">0.19</td>
<td align="right">65</td>
</tr>
<tr>
<td><code>s8_t681</code></td>
<td align="right">4,257,209</td>
<td align="right">4,266,438</td>
<td align="right">4,294,380</td>
<td align="right">0.65</td>
<td align="right">74</td>
<td align="right">3,883,493</td>
<td align="right">3,886,140</td>
<td align="right">3,886,140</td>
<td align="right">0</td>
<td align="right">71</td>
</tr>
<tr>
<td><code>s8_t694</code></td>
<td align="right">4,541,909</td>
<td align="right">4,553,863</td>
<td align="right">4,577,040</td>
<td align="right">0.51</td>
<td align="right">80</td>
<td align="right">4,270,748</td>
<td align="right">4,273,749</td>
<td align="right">4,286,700</td>
<td align="right">0.30</td>
<td align="right">77</td>
</tr>
<tr>
<td><code>s8_t734</code></td>
<td align="right">3,793,613</td>
<td align="right">3,803,805</td>
<td align="right">3,825,540</td>
<td align="right">0.57</td>
<td align="right">67</td>
<td align="right">3,516,953</td>
<td align="right">3,519,694</td>
<td align="right">3,526,980</td>
<td align="right">0.21</td>
<td align="right">63</td>
</tr>
<tr>
<td><code>s8_t872</code></td>
<td align="right">5,253,048</td>
<td align="right">5,265,660</td>
<td align="right">5,323,500</td>
<td align="right">1.09</td>
<td align="right">92</td>
<td align="right">4,904,474</td>
<td align="right">4,907,288</td>
<td align="right">4,924,980</td>
<td align="right">0.36</td>
<td align="right">86</td>
</tr>
<tr>
<td><code>s9_t773</code></td>
<td align="right">4,373,174</td>
<td align="right">4,384,561</td>
<td align="right">4,409,760</td>
<td align="right">0.57</td>
<td align="right">77</td>
<td align="right">4,054,312</td>
<td align="right">4,057,377</td>
<td align="right">4,064,340</td>
<td align="right">0.17</td>
<td align="right">73</td>
</tr>
<tr>
<td><code>s9_t775</code></td>
<td align="right">4,566,158</td>
<td align="right">4,580,470</td>
<td align="right">4,608,780</td>
<td align="right">0.61</td>
<td align="right">81</td>
<td align="right">4,212,572</td>
<td align="right">4,216,509</td>
<td align="right">4,232,580</td>
<td align="right">0.38</td>
<td align="right">76</td>
</tr>
<tr>
<td><code>s9_t784</code></td>
<td align="right">4,266,799</td>
<td align="right">4,275,539</td>
<td align="right">4,284,180</td>
<td align="right">0.20</td>
<td align="right">75</td>
<td align="right">3,982,069</td>
<td align="right">3,986,176</td>
<td align="right">3,992,460</td>
<td align="right">0.16</td>
<td align="right">72</td>
</tr>
<tr>
<td><code>s9_t946</code></td>
<td align="right">5,564,229</td>
<td align="right">5,572,249</td>
<td align="right">5,590,680</td>
<td align="right">0.33</td>
<td align="right">97</td>
<td align="right">5,256,955</td>
<td align="right">5,259,692</td>
<td align="right">5,272,380</td>
<td align="right">0.24</td>
<td align="right">95</td>
</tr>
<tr>
<td><code>s9_t972</code></td>
<td align="right">5,076,012</td>
<td align="right">5,083,015</td>
<td align="right">5,134,260</td>
<td align="right">1.00</td>
<td align="right">90</td>
<td align="right">4,768,967</td>
<td align="right">4,771,382</td>
<td align="right">4,787,940</td>
<td align="right">0.35</td>
<td align="right">86</td>
</tr>
<tr>
<td><code>s9_t991</code></td>
<td align="right">4,801,999</td>
<td align="right">4,809,359</td>
<td align="right">4,831,620</td>
<td align="right">0.46</td>
<td align="right">82</td>
<td align="right">4,480,773</td>
<td align="right">4,484,429</td>
<td align="right">4,507,920</td>
<td align="right">0.52</td>
<td align="right">79</td>
</tr>
<tr>
<td><code>s10_t928</code></td>
<td align="right">5,818,100</td>
<td align="right">5,831,520</td>
<td align="right">5,900,040</td>
<td align="right">1.16</td>
<td align="right">103</td>
<td align="right">5,213,343</td>
<td align="right">5,217,440</td>
<td align="right">5,235,000</td>
<td align="right">0.34</td>
<td align="right">96</td>
</tr>
<tr>
<td><code>s11_t961</code></td>
<td align="right">6,036,364</td>
<td align="right">6,046,847</td>
<td align="right">6,108,540</td>
<td align="right">1.01</td>
<td align="right">108</td>
<td align="right">5,236,197</td>
<td align="right">5,239,202</td>
<td align="right">5,256,000</td>
<td align="right">0.32</td>
<td align="right">97</td>
</tr>
<tr>
<td><code>s9_t1020</code></td>
<td align="right">5,656,977</td>
<td align="right">5,662,419</td>
<td align="right">5,694,780</td>
<td align="right">0.57</td>
<td align="right">97</td>
<td align="right">5,161,683</td>
<td align="right">5,165,267</td>
<td align="right">5,182,380</td>
<td align="right">0.33</td>
<td align="right">89</td>
</tr>
<tr>
<td><code>s10_t1014</code></td>
<td align="right">5,784,168</td>
<td align="right">5,793,198</td>
<td align="right">5,821,860</td>
<td align="right">0.49</td>
<td align="right">102</td>
<td align="right">5,415,092</td>
<td align="right">5,418,400</td>
<td align="right">5,432,940</td>
<td align="right">0.27</td>
<td align="right">98</td>
</tr>
<tr>
<td><code>s10_t1016</code></td>
<td align="right">5,722,362</td>
<td align="right">5,729,371</td>
<td align="right">5,770,740</td>
<td align="right">0.72</td>
<td align="right">101</td>
<td align="right">5,345,895</td>
<td align="right">5,348,589</td>
<td align="right">5,365,800</td>
<td align="right">0.32</td>
<td align="right">98</td>
</tr>
<tr>
<td><code>s10_t1088</code></td>
<td align="right">6,352,434</td>
<td align="right">6,363,921</td>
<td align="right">6,415,740</td>
<td align="right">0.81</td>
<td align="right">112</td>
<td align="right">5,804,036</td>
<td align="right">5,806,832</td>
<td align="right">5,826,240</td>
<td align="right">0.33</td>
<td align="right">103</td>
</tr>
<tr>
<td><code>s11_t1078</code></td>
<td align="right">6,694,088</td>
<td align="right">6,700,406</td>
<td align="right">6,735,120</td>
<td align="right">0.52</td>
<td align="right">116</td>
<td align="right">6,140,054</td>
<td align="right">6,142,352</td>
<td align="right">6,160,680</td>
<td align="right">0.30</td>
<td align="right">111</td>
</tr>
<tr>
<td><code>s11_t1151</code></td>
<td align="right">6,781,233</td>
<td align="right">6,790,106</td>
<td align="right">6,858,120</td>
<td align="right">0.99</td>
<td align="right">117</td>
<td align="right">6,158,369</td>
<td align="right">6,161,425</td>
<td align="right">6,173,640</td>
<td align="right">0.20</td>
<td align="right">111</td>
</tr>
<tr>
<td><code>s11_t1204</code></td>
<td align="right">6,532,036</td>
<td align="right">6,540,270</td>
<td align="right">6,582,900</td>
<td align="right">0.65</td>
<td align="right">114</td>
<td align="right">6,106,999</td>
<td align="right">6,109,832</td>
<td align="right">6,145,740</td>
<td align="right">0.58</td>
<td align="right">107</td>
</tr>
<tr>
<td><code>s12_t1049</code></td>
<td align="right">6,878,240</td>
<td align="right">6,889,604</td>
<td align="right">6,979,860</td>
<td align="right">1.29</td>
<td align="right">119</td>
<td align="right">5,718,836</td>
<td align="right">5,722,722</td>
<td align="right">5,742,660</td>
<td align="right">0.35</td>
<td align="right">104</td>
</tr>
<tr>
<td><code>s12_t1459</code></td>
<td align="right">7,570,579</td>
<td align="right">7,576,125</td>
<td align="right">7,637,520</td>
<td align="right">0.80</td>
<td align="right">131</td>
<td align="right">7,010,843</td>
<td align="right">7,012,799</td>
<td align="right">7,037,040</td>
<td align="right">0.34</td>
<td align="right">128</td>
</tr>
<tr>
<td><code>s12_t1482</code></td>
<td align="right">8,496,623</td>
<td align="right">8,502,321</td>
<td align="right">8,557,440</td>
<td align="right">0.64</td>
<td align="right">144</td>
<td align="right">7,623,706</td>
<td align="right">7,628,849</td>
<td align="right">7,664,520</td>
<td align="right">0.47</td>
<td align="right">132</td>
</tr>
<tr>
<td><code>s12_t1498</code></td>
<td align="right">7,951,231</td>
<td align="right">7,960,595</td>
<td align="right">8,040,960</td>
<td align="right">1.00</td>
<td align="right">136</td>
<td align="right">7,141,899</td>
<td align="right">7,145,873</td>
<td align="right">7,197,540</td>
<td align="right">0.72</td>
<td align="right">125</td>
</tr>
<tr>
<td><code>s13_t1286</code></td>
<td align="right">8,070,378</td>
<td align="right">8,079,261</td>
<td align="right">8,155,980</td>
<td align="right">0.94</td>
<td align="right">140</td>
<td align="right">7,056,461</td>
<td align="right">7,058,781</td>
<td align="right">7,090,320</td>
<td align="right">0.44</td>
<td align="right">124</td>
</tr>
<tr>
<td><code>s13_t1351</code></td>
<td align="right">6,856,205</td>
<td align="right">6,863,829</td>
<td align="right">6,915,240</td>
<td align="right">0.74</td>
<td align="right">120</td>
<td align="right">6,247,774</td>
<td align="right">6,249,757</td>
<td align="right">6,271,560</td>
<td align="right">0.35</td>
<td align="right">112</td>
</tr>
<tr>
<td><code>s13_t1372</code></td>
<td align="right">8,350,945</td>
<td align="right">8,361,823</td>
<td align="right">8,459,580</td>
<td align="right">1.16</td>
<td align="right">146</td>
<td align="right">7,452,535</td>
<td align="right">7,454,846</td>
<td align="right">7,474,860</td>
<td align="right">0.27</td>
<td align="right">135</td>
</tr>
<tr>
<td><code>s13_t1532</code></td>
<td align="right">9,050,466</td>
<td align="right">9,056,799</td>
<td align="right">9,115,680</td>
<td align="right">0.65</td>
<td align="right">154</td>
<td align="right">8,128,086</td>
<td align="right">8,130,272</td>
<td align="right">8,160,240</td>
<td align="right">0.37</td>
<td align="right">146</td>
</tr>
<tr>
<td><code>s13_t1591</code></td>
<td align="right">8,716,345</td>
<td align="right">8,720,590</td>
<td align="right">8,757,720</td>
<td align="right">0.42</td>
<td align="right">153</td>
<td align="right">8,246,490</td>
<td align="right">8,248,519</td>
<td align="right">8,269,680</td>
<td align="right">0.26</td>
<td align="right">152</td>
</tr>
<tr>
<td><code>s13_t1598</code></td>
<td align="right">8,590,185</td>
<td align="right">8,596,695</td>
<td align="right">8,664,360</td>
<td align="right">0.78</td>
<td align="right">149</td>
<td align="right">7,670,143</td>
<td align="right">7,672,742</td>
<td align="right">7,706,700</td>
<td align="right">0.44</td>
<td align="right">139</td>
</tr>
<tr>
<td><code>s14_t1500</code></td>
<td align="right">8,835,895</td>
<td align="right">8,845,046</td>
<td align="right">8,880,420</td>
<td align="right">0.40</td>
<td align="right">154</td>
<td align="right">8,222,074</td>
<td align="right">8,224,192</td>
<td align="right">8,245,860</td>
<td align="right">0.26</td>
<td align="right">150</td>
</tr>
<tr>
<td><code>s14_t1511</code></td>
<td align="right">9,167,303</td>
<td align="right">9,173,645</td>
<td align="right">9,257,400</td>
<td align="right">0.90</td>
<td align="right">157</td>
<td align="right">7,817,050</td>
<td align="right">7,818,507</td>
<td align="right">7,838,760</td>
<td align="right">0.26</td>
<td align="right">144</td>
</tr>
<tr>
<td><code>s14_t1629</code></td>
<td align="right">10,146,016</td>
<td align="right">10,151,858</td>
<td align="right">10,212,780</td>
<td align="right">0.60</td>
<td align="right">177</td>
<td align="right">8,333,186</td>
<td align="right">8,335,086</td>
<td align="right">8,358,000</td>
<td align="right">0.27</td>
<td align="right">149</td>
</tr>
<tr>
<td><code>s14_t1755</code></td>
<td align="right">10,283,388</td>
<td align="right">10,289,863</td>
<td align="right">10,356,000</td>
<td align="right">0.64</td>
<td align="right">176</td>
<td align="right">9,408,259</td>
<td align="right">9,409,947</td>
<td align="right">9,432,780</td>
<td align="right">0.24</td>
<td align="right">170</td>
</tr>
<tr>
<td><code>s15_t1713</code></td>
<td align="right">10,034,985</td>
<td align="right">10,041,287</td>
<td align="right">10,130,340</td>
<td align="right">0.88</td>
<td align="right">172</td>
<td align="right">8,823,104</td>
<td align="right">8,825,561</td>
<td align="right">8,869,920</td>
<td align="right">0.50</td>
<td align="right">156</td>
</tr>
<tr>
<td><code>s15_t1745</code></td>
<td align="right">10,366,864</td>
<td align="right">10,372,707</td>
<td align="right">10,458,720</td>
<td align="right">0.82</td>
<td align="right">177</td>
<td align="right">9,112,295</td>
<td align="right">9,114,199</td>
<td align="right">9,140,520</td>
<td align="right">0.29</td>
<td align="right">164</td>
</tr>
<tr>
<td><code>s15_t1749</code></td>
<td align="right">9,308,113</td>
<td align="right">9,312,168</td>
<td align="right">9,372,480</td>
<td align="right">0.64</td>
<td align="right">162</td>
<td align="right">8,622,494</td>
<td align="right">8,624,236</td>
<td align="right">8,653,620</td>
<td align="right">0.34</td>
<td align="right">158</td>
</tr>
<tr>
<td><code>s17_t1955</code></td>
<td align="right">11,758,675</td>
<td align="right">11,766,551</td>
<td align="right">11,854,920</td>
<td align="right">0.75</td>
<td align="right">204</td>
<td align="right">10,117,389</td>
<td align="right">10,119,161</td>
<td align="right">10,152,660</td>
<td align="right">0.33</td>
<td align="right">186</td>
</tr>
<tr>
<td><code>s15_t2029</code></td>
<td align="right">11,134,303</td>
<td align="right">11,140,680</td>
<td align="right">11,257,260</td>
<td align="right">1.04</td>
<td align="right">190</td>
<td align="right">9,917,645</td>
<td align="right">9,919,298</td>
<td align="right">9,960,660</td>
<td align="right">0.42</td>
<td align="right">177</td>
</tr>
<tr>
<td><code>s16_t2052</code></td>
<td align="right">11,938,880</td>
<td align="right">11,944,278</td>
<td align="right">12,045,540</td>
<td align="right">0.84</td>
<td align="right">203</td>
<td align="right">10,468,828</td>
<td align="right">10,470,472</td>
<td align="right">10,514,220</td>
<td align="right">0.42</td>
<td align="right">187</td>
</tr>
<tr>
<td><code>s16_t2136</code></td>
<td align="right">12,715,984</td>
<td align="right">12,719,602</td>
<td align="right">12,788,520</td>
<td align="right">0.54</td>
<td align="right">217</td>
<td align="right">11,405,783</td>
<td align="right">11,406,933</td>
<td align="right">11,446,920</td>
<td align="right">0.35</td>
<td align="right">209</td>
</tr>
<tr>
<td><code>s16_t2219</code></td>
<td align="right">13,318,246</td>
<td align="right">13,324,371</td>
<td align="right">13,437,960</td>
<td align="right">0.85</td>
<td align="right">227</td>
<td align="right">10,702,291</td>
<td align="right">10,703,286</td>
<td align="right">10,741,800</td>
<td align="right">0.36</td>
<td align="right">195</td>
</tr>
<tr>
<td><code>s16_t2252</code></td>
<td align="right">12,396,038</td>
<td align="right">12,400,856</td>
<td align="right">12,535,440</td>
<td align="right">1.07</td>
<td align="right">214</td>
<td align="right">11,064,280</td>
<td align="right">11,065,751</td>
<td align="right">11,118,060</td>
<td align="right">0.47</td>
<td align="right">200</td>
</tr>
<tr>
<td><code>s17_t2090</code></td>
<td align="right">12,436,106</td>
<td align="right">12,441,737</td>
<td align="right">12,525,420</td>
<td align="right">0.67</td>
<td align="right">212</td>
<td align="right">10,852,090</td>
<td align="right">10,853,424</td>
<td align="right">10,891,680</td>
<td align="right">0.35</td>
<td align="right">197</td>
</tr>
<tr>
<td><code>s17_t2166</code></td>
<td align="right">14,037,157</td>
<td align="right">14,044,780</td>
<td align="right">14,128,740</td>
<td align="right">0.59</td>
<td align="right">238</td>
<td align="right">11,642,240</td>
<td align="right">11,643,649</td>
<td align="right">11,681,700</td>
<td align="right">0.33</td>
<td align="right">214</td>
</tr>
<tr>
<td><code>s17_t2183</code></td>
<td align="right">14,290,908</td>
<td align="right">14,297,875</td>
<td align="right">14,451,960</td>
<td align="right">1.07</td>
<td align="right">244</td>
<td align="right">12,328,601</td>
<td align="right">12,331,002</td>
<td align="right">12,381,840</td>
<td align="right">0.41</td>
<td align="right">219</td>
</tr>
<tr>
<td><code>s17_t2214</code></td>
<td align="right">12,387,240</td>
<td align="right">12,391,876</td>
<td align="right">12,441,960</td>
<td align="right">0.40</td>
<td align="right">216</td>
<td align="right">10,657,805</td>
<td align="right">10,659,956</td>
<td align="right">10,720,080</td>
<td align="right">0.56</td>
<td align="right">187</td>
</tr>
<tr>
<td><code>s17_t2242</code></td>
<td align="right">14,742,098</td>
<td align="right">14,748,939</td>
<td align="right">14,952,300</td>
<td align="right">1.36</td>
<td align="right">256</td>
<td align="right">12,606,446</td>
<td align="right">12,608,013</td>
<td align="right">12,650,520</td>
<td align="right">0.34</td>
<td align="right">229</td>
</tr>
<tr>
<td><code>s17_t2366</code></td>
<td align="right">13,478,416</td>
<td align="right">13,483,797</td>
<td align="right">13,620,840</td>
<td align="right">1.01</td>
<td align="right">234</td>
<td align="right">11,891,063</td>
<td align="right">11,892,482</td>
<td align="right">11,931,600</td>
<td align="right">0.33</td>
<td align="right">218</td>
</tr>
<tr>
<td><code>s18_t2395</code></td>
<td align="right">15,425,380</td>
<td align="right">15,429,645</td>
<td align="right">15,542,940</td>
<td align="right">0.73</td>
<td align="right">263</td>
<td align="right">13,764,435</td>
<td align="right">13,765,215</td>
<td align="right">13,799,940</td>
<td align="right">0.25</td>
<td align="right">249</td>
</tr>
<tr>
<td><code>s18_t2550</code></td>
<td align="right">14,939,689</td>
<td align="right">14,944,106</td>
<td align="right">15,041,760</td>
<td align="right">0.65</td>
<td align="right">257</td>
<td align="right">13,480,955</td>
<td align="right">13,481,910</td>
<td align="right">13,541,220</td>
<td align="right">0.44</td>
<td align="right">243</td>
</tr>
<tr>
<td><code>s18_t2595</code></td>
<td align="right">13,723,693</td>
<td align="right">13,728,804</td>
<td align="right">13,837,860</td>
<td align="right">0.79</td>
<td align="right">234</td>
<td align="right">12,149,343</td>
<td align="right">12,150,418</td>
<td align="right">12,199,080</td>
<td align="right">0.40</td>
<td align="right">223</td>
</tr>
<tr>
<td><code>s18_t2641</code></td>
<td align="right">15,474,385</td>
<td align="right">15,478,417</td>
<td align="right">15,627,720</td>
<td align="right">0.96</td>
<td align="right">265</td>
<td align="right">13,458,876</td>
<td align="right">13,459,831</td>
<td align="right">13,528,980</td>
<td align="right">0.51</td>
<td align="right">237</td>
</tr>
<tr>
<td><code>s18_t2648</code></td>
<td align="right">13,801,297</td>
<td align="right">13,806,594</td>
<td align="right">13,921,500</td>
<td align="right">0.83</td>
<td align="right">234</td>
<td align="right">12,094,401</td>
<td align="right">12,095,027</td>
<td align="right">12,150,300</td>
<td align="right">0.45</td>
<td align="right">218</td>
</tr>
<tr>
<td><code>s19_t2315</code></td>
<td align="right">14,810,475</td>
<td align="right">14,817,684</td>
<td align="right">14,958,960</td>
<td align="right">0.94</td>
<td align="right">253</td>
<td align="right">12,585,061</td>
<td align="right">12,586,784</td>
<td align="right">12,633,420</td>
<td align="right">0.37</td>
<td align="right">225</td>
</tr>
<tr>
<td><code>s19_t2484</code></td>
<td align="right">15,219,679</td>
<td align="right">15,225,464</td>
<td align="right">15,369,840</td>
<td align="right">0.94</td>
<td align="right">261</td>
<td align="right">12,461,767</td>
<td align="right">12,463,222</td>
<td align="right">12,537,360</td>
<td align="right">0.59</td>
<td align="right">226</td>
</tr>
<tr>
<td><code>s19_t2661</code></td>
<td align="right">18,565,600</td>
<td align="right">18,571,086</td>
<td align="right">18,741,660</td>
<td align="right">0.91</td>
<td align="right">317</td>
<td align="right">14,820,822</td>
<td align="right">14,821,928</td>
<td align="right">14,882,040</td>
<td align="right">0.40</td>
<td align="right">269</td>
</tr>
<tr>
<td><code>s19_t2702</code></td>
<td align="right">14,331,231</td>
<td align="right">14,335,649</td>
<td align="right">14,423,520</td>
<td align="right">0.61</td>
<td align="right">247</td>
<td align="right">12,840,737</td>
<td align="right">12,840,737</td>
<td align="right">12,911,940</td>
<td align="right">0.55</td>
<td align="right">233</td>
</tr>
<tr>
<td><code>s19_t2711</code></td>
<td align="right">15,915,564</td>
<td align="right">15,919,393</td>
<td align="right">15,988,620</td>
<td align="right">0.43</td>
<td align="right">270</td>
<td align="right">14,476,229</td>
<td align="right">14,477,151</td>
<td align="right">14,533,020</td>
<td align="right">0.38</td>
<td align="right">258</td>
</tr>
<tr>
<td><code>s19_t2744</code></td>
<td align="right">15,100,876</td>
<td align="right">15,104,590</td>
<td align="right">15,214,140</td>
<td align="right">0.72</td>
<td align="right">259</td>
<td align="right">13,331,065</td>
<td align="right">13,331,810</td>
<td align="right">13,382,700</td>
<td align="right">0.38</td>
<td align="right">243</td>
</tr>
<tr>
<td><code>s20_t2668</code></td>
<td align="right">15,799,233</td>
<td align="right">15,802,963</td>
<td align="right">15,861,120</td>
<td align="right">0.37</td>
<td align="right">274</td>
<td align="right">13,605,974</td>
<td align="right">13,606,853</td>
<td align="right">13,665,660</td>
<td align="right">0.43</td>
<td align="right">253</td>
</tr>
<tr>
<td><code>s20_t2921</code></td>
<td align="right">18,007,663</td>
<td align="right">18,011,628</td>
<td align="right">18,133,260</td>
<td align="right">0.67</td>
<td align="right">310</td>
<td align="right">15,992,132</td>
<td align="right">15,993,143</td>
<td align="right">16,076,100</td>
<td align="right">0.52</td>
<td align="right">291</td>
</tr>
<tr>
<td><code>s20_t3016</code></td>
<td align="right">16,181,075</td>
<td align="right">16,184,454</td>
<td align="right">16,287,780</td>
<td align="right">0.63</td>
<td align="right">277</td>
<td align="right">14,703,742</td>
<td align="right">14,704,066</td>
<td align="right">14,756,220</td>
<td align="right">0.35</td>
<td align="right">265</td>
</tr>
</tbody>
</table>
