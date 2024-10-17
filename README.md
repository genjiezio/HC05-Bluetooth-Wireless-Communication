# Getting-start

Please read the "蓝牙模块通信操作说明.pdf" 


I'll add the version of English soon later.

# 使用前1000个新闻来创建corpus和texts
temp_News_sample = News_sample.head(1000)
# 将结果添加到DataFrame中
temp_News_sample['Fin_polarity'] = polarity
temp_News_sample['snow_polarity'] = temp_News_sample['NewsContent'].apply(lambda x: SnowNLP(x).sentiments)
