# ML100-Days
機器學習百日馬拉松

Day 1: 當我們遇到一個問題時，不見得要馬上跳進去玩耍；
	
	我們要先思考問題，知道目的，如果有資料，還可以概略看一下資料，盤算能夠作出甚麼有趣有用的結果。
	如果沒有資料，就問題的思考後，才去採集資料，相對可以節省很多時間。
	
	之後我們才會盤算一個策略去進行行動，比如快速完成一個方案，一個最小可行方案(Minimum Visiable Product 的概念)，後續進行優化改善。
	
	HW: 除了第一天的簡易練習 編寫 Y=wX+b，plot(X,Y) 定義 mse, mae 還有一個很重要的工作，作業2：如果你今天經營一個台灣大車隊，你要如何透過數據分析來提升業績? 思考一下，我們除了需要工程師也需要資料分析師與科學家。


Day 2: 第一次資料探勘

	好我們前十六天都將進行資料數據前處理的工作，練習的問題會是 Kaggle 上的題目 
	https://www.kaggle.com/c/home-credit-default-risk/data 
	
	會用到的應該是 application_train.csv 與 application_test.csv 
	最後要上傳時會用到 submission.csv 
	但是請不要忘了研讀 HomeCredit_columns_description.csv 
	
	HW:
	第二天我們開始讀取資料，對於這個被整理好的 Dataframe 進行最初步的探勘，比如說知道有多少筆資料，有多少 "欄" 的特徵，如何將特徵項目組成一個 list， 又或者我們該如何呈現截取部分資料等。總之，我們還沒有跳進去觀察個別特徵，個別資料前，我們所採取的動作在今天試著作一輪。
	第二天還有一個有趣的參考作業，讀一讀吳老師的資料探勘講義，其中為何要研究杜河的魚類又如何進行都是很有意義的練習，川普的故事也趣味十足。
	
Day 3: 關於 DataFrame
	
	我們在作資料清理，在處理機器學習的問題時，常常都要熟練 DataFrame 的操作，DataFrame 就像是 EXCEL 的 Spreadsheet 一樣，第一列存著的是所有欄位名稱，就是我們未來要處理的特徵。第二列起就是一筆一筆的資料。
	
	HW: 第三天的練習會比 pandas 的 DataFrame 多一點不同格式的東西，大家好好努力!
	
Day 4: EDA 資料類型介紹

	我們在第二天開始進行了 EDA 資料探勘的動作，當時是看整個資料的外型，有多少特徵有多少筆資料，今天起我們要開始一步一步的觀察特徵資料。
	
	跳進特徵研究的第一個小動作就是要知道，每一個特徵的格式，也就是資料的類別；基本的類別有 float64, int64, object。
	
	要留意 object是我們的機器無法直接處理的資料類型，所以今天是介紹為這類資料作編碼，編碼完後才會送進機器模型運算。
	
	HW: 請研讀參考資料 https://medium.com/@contactsunny/label-encoder-vs-one-hot-encoder-in-machine-learning-3fc273365621
	，同時完成第四天的程式。
	
Day 5: EDA之資料分布

	EDA 當然沒有固定的程序進行，但是對於新手而言，對於十個出頭的特徵的經典題目 Titanic 都已經是不知道如何下手了，更何況今天的題目有百餘個特徵。所以如果有一個按部就班的程序可以遵循，在新手時期是十分珍貴的。
	
	今天算是第三天的 EDA，Day 2時是第一次看資料框架(有多少資料，是寬的胖的高的瘦的)，Day 4 時是觀察這些特徵的資料類型，今天我們要來看看特徵資料的統計特性，
	計算集中趨勢
		•平均值 Mean
		•中位數 Median
		•眾數 Mode 
	計算資料分散程度
		•最⼩值 Min
		•最⼤值 Max
		•範圍 Range
		•四分位差 Quartiles
		•變異數 Variance
		•標準差 Standard deviation
		
	HW: 今天的作業是挑三個有興趣的特徵來看它們的統計特性，挑選的方式可以是在 Day 2時的 HomeCredit_columns_description.csv 研讀時對於特徵了解而挑選，如果挑很多個，最後也可以用 sns.heatmap(corr()matric) 的關係來挑選。
	
	
	
	
	
	
