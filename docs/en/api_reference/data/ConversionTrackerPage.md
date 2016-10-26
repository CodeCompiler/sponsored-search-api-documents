# ConversionTrackerPage
ConversionTrackerPage object shows entry of ConversionTracker.
### Service
+ [ConversionTrackerService](../services/ConversionTrackerService.md)

| Field | Data Type | Description | 
|---|---|---|
| Page(inherited)|||
| totalNumEntries| xsd:int| Total number of entries |
| ConversionTrackerPage|||
| totalNumConvertedClicks| xsd:long| Sum of Click through Conversion. <br>*This data item has been disabled as of October 26, 2016.<br>All return values will be "0" (zero).|
| totalNumConversionEvents| xsd:long| Sum of the number of Conversion event |
| totalConversionValue| xsd:long| Sum of the value of Conversion |
| values[]| <a href="./ConversionTrackerValues.md">ConversionTrackerValues</a>| ConversionTracker information |
<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
