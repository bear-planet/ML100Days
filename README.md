# ◆ --- 機器學習百日馬拉松 Homework & Note --- ◆

<h2> √ D1：資料介紹與評估資料  </h2>
<h2> √ D2：機器學習概論       </h2>
<h2> √ D3：機器學習-流程與步驟      </h2>
<h2> √ D4：EDA (Exploratory Data Analysis)/讀取資料與分析流程       </h2>
<h2> √ D5：如何新建一個Dataframe? 如何讀取其他資料?(非csv的資料)       </h2>
<h2> √ D6：EDA:欄位的資料類型介紹及處理       </h2>

<h2> √ D7：特徵類型    </h2>
<h3> ｜常見的特徵類型  </h3> 
  <h5> ◆ 數值型特徵, EX: 坪數、年齡 </h5>
  <h5> ◆ 類別型特徵, EX: 行政區、性別 </h5>
   
<h3> ｜交叉驗證(Cross Validatioin) </h3>
  <h5> ◇ The Validation Set Approach </h5>
  <h5> ◇ LOOCV （Leave-one-out cross-validation） </h5>
  <h5> ◇ K-fold Cross Validation </h5>
  

<h2> √ D8：EDA資料分佈    </h2>
<h2> √ D9：EDA：離群值(Outliner)及其處理    </h2>
<h3> ｜檢查異常值的方法 </h3>
  <h5> ◇ 視覺方法 - boxplot, scatter plot </h5>
  <h5>    ◇  統計方法 - zscore, IQR  </h5>
  
<h2> √ D10 : 數值型特徵 - 去除離群值 </h2>
<h2> √ D11 常用的數值取代：中位數與分位數連續數值標準化 </h2>
<h3> ｜常用以填補的統計值 </h3>

| 常用以填補的統計值 | 方法     |
| --- | --- |
| **中位數(median)** | np.median(value_array) |
| **分位數(quantiles)** | np.quantile(value_array, q = ... ) |
| **眾數(mode)** | dictionary method :較快的方法 |
| 平均數(mean) | np.mean(value_array) |

<h2> √ D12 數值型特徵-補缺失值與標準化 </h2>
<h3> ｜標準化 / 最小最大化適用場合 </h3>

| model | 例子 |
| --- | --- |
| 非樹狀模型 | 如線性迴歸, 羅吉斯迴歸, 類神經...等，標準化 / 最小最大化後對預測**會有影響** |
| 樹狀模型 | 如決策樹, 隨機森林, 梯度提升樹...等，標準化 / 最小最大化後對預測**不會有影響** |

<h2> √ D13 DataFrame operationData frame merge/常用的 DataFrame 操作 </h2>
<h2> √ D14 程式實作 EDA: correlation/相關係數簡介 </h2>
<h2> √ D15 EDA from Correlation </h2>
<h2> √ D16 EDA: 不同數值範圍間的特徵如何檢視/繪圖與樣式Kernel Density Estimation (KDE) </h2>

<h3> ｜繪圖風格 </h3>

| 繪圖風格 | 語法 |
| --- | --- |
| default | plt.style.use(‘default’) # 不需設定就會使用預設 |
| ggplot | plt.style.use('ggplot') |
| seaborn | plt.style.use(‘seaborn’) # 或採用 seaborn 套件繪圖 |

<h3> ｜何謂 核密度估計 Kernel Density Estimation (KDE) </h3>
<h4> ✻ [KDE](https://blog.csdn.net/unixtch/article/details/78556499) </h4>
<h4> ✻ [簡單說：把長條圖畫成折線圖！](https://reurl.cc/R6Dmp9) </h4>

<h2> √ D17 EDA: 把連續型變數離散化 </h2>
<h3> ｜NOTE </h3>
  <h5> ◆ 離散化的目的是讓事情變簡單、減少 outlier 對分析以及訓練模型的影響 </h5>
  <h5> ◆ 主要的方法是等寬劃分 (對應 pandas 中的 cut) 以及等頻劃分 (對應 pandas 中的 qcut) </h5>
  <h5> ◆ 可以依實際需求來自己定義離散化的方式 </h5>
  
<h3> ｜延伸閱讀 </h3>
<h4> ✻ [連續特徵的離散化 : 在什麼情況下可以獲得更好的效果?](https://www.zhihu.com/question/31989952) </h4>

<h2> √ D18 程式實作 把連續型變數離散化 </h2>
<h2> √ D19 Subplots </h2>
<h3> ｜延伸閱讀 </h3>
<h4> ✻ [matplotlib 官方範例](https://matplotlib.org/2.0.2/examples/pylab_examples/subplots_demo.html) </h4>
<h4> ✻ [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/04.08-multiple-subplots.html) </h4>
<h4> ✻ [另類子圖 Seaborn.jointplot](https://seaborn.pydata.org/generated/seaborn.jointplot.html) </h4>

<h2> √ D20 Heatmap & Grid-plot </h2>
<h3> ｜NOTE </h3>
  <h5> ◆ Heatmap 常用於呈現訊息的強弱 (以顏色深淺呈現)，也常用於呈現混淆矩陣 </h5>
  <h5> ◆ pair/gridplot 結合了 scatter plot 與 historgram 的好處來呈現變數間的相關程度 </h5>
  
<h3> ｜延伸閱讀 </h3>
<h4> ✻ [Heatmap](https://matplotlib.org/3.2.2/gallery/images_contours_and_fields/image_annotated_heatmap.html) </h4>
<h4> ✻ [Pairplot 的更多應用實例](https://towardsdatascience.com/visualizing-data-with-pair-plots-in-python-f228cf529166) </h4>

<h2> √ D24：類別型特徵 - 基礎處理 </h2>
<h3> ｜NOTE </h3>
  <h5> ◆ 類別型特徵有標籤編碼 (Label Encoding) 與獨熱編碼 (One Hot Encoding) 兩種基礎編碼方式 </h5>
  <h5> ◆ 兩種編碼中標籤編碼比較常用 </h5>
  <h5> ◆ 當特徵重要性高，且可能值較少時，才應該考慮獨熱編碼 </h5>



     
