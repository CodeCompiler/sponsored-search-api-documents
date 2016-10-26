# ConversionTracker
ConversionTracker object shows ConversionTracker information such as ConversionTag and performance data by tag.
### Service
+ [ConversionTrackerService](../services/ConversionTrackerService.md)

| Field | Data Type | Description | ADD | SET | 
|---|---|---|---|---|
| accountId| xsd:long| Account ID| Req| Req |
| conversionTrackerId| xsd:long| ConversionTracker ID| -| Req |
| conversionTrackerName| xsd:string| ConversionTracker Name| Req| Opt |
| status| enum <a href="./ConversionTrackerStatus.md">ConversionTrackerStatus</a>| ConversionTracker Status| Req| Opt |
| category| enum <a href="./ConversionTrackerCategory.md">ConversionTrackerCategory</a>| Conversion category for tracking. Please specify a purpose for conversion from ConversionTrackerCategory.<br>* In the case of Call conversion, PAGE_VEIW is not specifiable.<br>* In the case of App conversion, DEFAULT is only specifiable.| Req| Opt |
| numConversionEvents| xsd:int| Total conversions.<br>Total conversions are the count for all conversions that resulted within 30 days of 1 click of an ad.| -| - |
| conversionValue| xsd:long| Total sales by conversion.| -| - |
| mostRecentConversionDate| xsd:string| Most recent date of Conversion| -| - |
| numConvertedClicks| xsd:int| The number of Unique Conversions.<br>The unique conversion refers to the first conversion that resulted within 30 days of 1 click of an ad.<br>Even if several conversions resulted from a click of an ad, the second and further conversions are not counted.<br>*This data item has been disabled as of October 26, 2016.<br>All return values will be "0" (zero).| -| - |
| conversionTrackerType| enum <a href="./ConversionTrackerType.md">ConversionTrackerType</a>| Conversion Type| Req| Req |
| userRevenueValue| xsd:string| Revenue value for ConversionTracker.<br>If fixed value is set for a conversion by user, total revenue is appeared in the report.<br>App conversion value is not assignable, download sales will be calculated as conversion value.<br>If the number is not set during the ADD request, it will be set 0 as default.| Opt| Opt |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
