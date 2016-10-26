# ConversionTracker
ConversionTrackerオブジェクトは、コンバージョン測定タグやタグごとのパフォーマンスデータなどのコンバージョントラッカー情報を表します。
### Service
+ [ConversionTrackerService](../services/ConversionTrackerService.md)

| フィールド | データ型 | 説明 | ADD | SET | 
|---|---|---|---|---|
| accountId| xsd:long| アカウントIDです。| Req| Req |
| conversionTrackerId| xsd:long| コンバージョントラッカーのIDです。| ─| Req |
| conversionTrackerName| xsd:string| コンバージョントラッカーの名称です。| Req| Opt |
| status| enum <a href="./ConversionTrackerStatus.md">ConversionTrackerStatus</a>| コンバージョントラッカーのステータスです。| Req| Opt |
| category| enum <a href="./ConversionTrackerCategory.md">ConversionTrackerCategory</a>| トラッキング対象のコンバージョンのカテゴリです。<br>コンバージョン測定を行う目的をConversionTrackerCategoryより選んでください。<br>※電話コンバージョンの場合は、PAGE_VEIWの指定はできません。<br>※アプリコンバージョンの場合は、DEFAULTのみ指定可能です。| Req| Opt |
| numConversionEvents| xsd:int| 総コンバージョン数です。広告1回のクリックに対して30日以内に発生したコンバージョンをすべてカウントします。| ─| ─ |
| conversionValue| xsd:long| コンバージョンの値です。| ─| ─ |
| mostRecentConversionDate| xsd:string| 直近のコンバージョン発生日です。| ─| ─ |
| numConvertedClicks| xsd:int| ユニークコンバージョン数です。<br>広告1回のクリックに対して30日以内に発生した全コンバージョン数のうち、最初の1回のみがカウントされます。<br>広告1回のクリックに対し複数のコンバージョンが発生しても、2回目以降のコンバージョン数はカウントされません。<br>※2016年10月26日をもちまして、本項目の値は取得できなくなりました。<br>すべて「0」が返却されます。| ─| ─ |
| conversionTrackerType| enum <a href="./ConversionTrackerType.md">ConversionTrackerType</a>| コンバージョンタイプです。| Req| Req |
| userRevenueValue| xsd:string| このコンバージョントラッカーに対するユーザー指定の収益値です。<br>1コンバージョンあたりの売上金額が固定値の場合、その金額を設定することで、売上金額をレポートなどで確認できます。<br>ADDリクエスト時に未指定の場合、0が設定されます。| Opt| Opt |
<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
