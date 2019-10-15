# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [AbortBuildPayload](#abortbuildpayload)
    * [Account](#account)
    * [AccountConnection](#accountconnection)
    * [AccountEdge](#accountedge)
    * [AuthToken](#authtoken)
    * [Build](#build)
    * [BuildConnection](#buildconnection)
    * [BuildEdge](#buildedge)
    * [CancelBuildPayload](#cancelbuildpayload)
    * [Crawl](#crawl)
    * [CrawlConnection](#crawlconnection)
    * [CrawlEdge](#crawledge)
    * [CrawlSegment](#crawlsegment)
    * [CrawlSegmentConnection](#crawlsegmentconnection)
    * [CrawlSegmentEdge](#crawlsegmentedge)
    * [CrawlUrl](#crawlurl)
    * [CrawlUrlConnection](#crawlurlconnection)
    * [CrawlUrlEdge](#crawlurledge)
    * [CreateBuildPayload](#createbuildpayload)
    * [CreateSegmentPayload](#createsegmentpayload)
    * [CreateTestPayload](#createtestpayload)
    * [CreateTestResultPayload](#createtestresultpayload)
    * [CreateTestSuitePayload](#createtestsuitepayload)
    * [CustomDnsSetting](#customdnssetting)
    * [DeleteSegmentPayload](#deletesegmentpayload)
    * [DeleteTestPayload](#deletetestpayload)
    * [DeleteTestSuitePayload](#deletetestsuitepayload)
    * [FeatureFlag](#featureflag)
    * [FinishBuildPayload](#finishbuildpayload)
    * [Location](#location)
    * [LocationConnection](#locationconnection)
    * [LocationEdge](#locationedge)
    * [PageInfo](#pageinfo)
    * [PredicateMetadata](#predicatemetadata)
    * [Project](#project)
    * [ProjectConnection](#projectconnection)
    * [ProjectEdge](#projectedge)
    * [ProjectUploadType](#projectuploadtype)
    * [Redirect](#redirect)
    * [Report](#report)
    * [ReportConnection](#reportconnection)
    * [ReportEdge](#reportedge)
    * [ReportTemplate](#reporttemplate)
    * [ReportTemplateConnection](#reporttemplateconnection)
    * [ReportTemplateEdge](#reporttemplateedge)
    * [RunBuildPayload](#runbuildpayload)
    * [Segment](#segment)
    * [SegmentConnection](#segmentconnection)
    * [SegmentEdge](#segmentedge)
    * [SegmentRule](#segmentrule)
    * [SegmentableMetricMetadata](#segmentablemetricmetadata)
    * [Test](#test)
    * [TestConnection](#testconnection)
    * [TestEdge](#testedge)
    * [TestResult](#testresult)
    * [TestResultConnection](#testresultconnection)
    * [TestResultEdge](#testresultedge)
    * [TestSuite](#testsuite)
    * [TestSuiteConnection](#testsuiteconnection)
    * [TestSuiteEdge](#testsuiteedge)
    * [UpdateTestPayload](#updatetestpayload)
    * [UpdateTestSuitePayload](#updatetestsuitepayload)
    * [User](#user)
    * [UserConnection](#userconnection)
    * [UserEdge](#useredge)
  * [Inputs](#inputs)
    * [AbortBuildInput](#abortbuildinput)
    * [AccountFilter](#accountfilter)
    * [AccountOrder](#accountorder)
    * [BuildFilter](#buildfilter)
    * [BuildOrder](#buildorder)
    * [CancelBuildInput](#cancelbuildinput)
    * [CrawlFilter](#crawlfilter)
    * [CrawlOrder](#crawlorder)
    * [CrawlSegmentFilter](#crawlsegmentfilter)
    * [CrawlSegmentOrder](#crawlsegmentorder)
    * [CrawlUrlFilter](#crawlurlfilter)
    * [CrawlUrlOrder](#crawlurlorder)
    * [CreateBuildInput](#createbuildinput)
    * [CreateSegmentInput](#createsegmentinput)
    * [CreateSegmentRuleInput](#createsegmentruleinput)
    * [CreateTestInput](#createtestinput)
    * [CreateTestResultInput](#createtestresultinput)
    * [CreateTestSuiteInput](#createtestsuiteinput)
    * [CustomDnsSettingInput](#customdnssettinginput)
    * [DeleteSegmentInput](#deletesegmentinput)
    * [DeleteTestInput](#deletetestinput)
    * [DeleteTestSuiteInput](#deletetestsuiteinput)
    * [FinishBuildInput](#finishbuildinput)
    * [LocationFilter](#locationfilter)
    * [LocationOrder](#locationorder)
    * [ProjectFilter](#projectfilter)
    * [ProjectOrder](#projectorder)
    * [ReportFilter](#reportfilter)
    * [ReportOrder](#reportorder)
    * [ReportTemplateFilter](#reporttemplatefilter)
    * [ReportTemplateOrder](#reporttemplateorder)
    * [RunBuildInput](#runbuildinput)
    * [SegmentFilter](#segmentfilter)
    * [SegmentOrder](#segmentorder)
    * [TestFilter](#testfilter)
    * [TestOrder](#testorder)
    * [TestResultFilter](#testresultfilter)
    * [TestResultOrder](#testresultorder)
    * [TestSuiteFilter](#testsuitefilter)
    * [TestSuiteOrder](#testsuiteorder)
    * [UpdateTestInput](#updatetestinput)
    * [UpdateTestSuiteInput](#updatetestsuiteinput)
    * [UserFilter](#userfilter)
    * [UserOrder](#userorder)
  * [Enums](#enums)
    * [AccountOrderField](#accountorderfield)
    * [BuildOrderField](#buildorderfield)
    * [BuildStatus](#buildstatus)
    * [CrawlOrderField](#crawlorderfield)
    * [CrawlSegmentOrderField](#crawlsegmentorderfield)
    * [CrawlUrlOrderField](#crawlurlorderfield)
    * [LocationCode](#locationcode)
    * [LocationOrderField](#locationorderfield)
    * [OrderDirection](#orderdirection)
    * [Predicate](#predicate)
    * [PrimitiveType](#primitivetype)
    * [ProjectOrderField](#projectorderfield)
    * [ReportOrderField](#reportorderfield)
    * [ReportTemplateOrderField](#reporttemplateorderfield)
    * [SegmentOrderField](#segmentorderfield)
    * [SegmentableMetric](#segmentablemetric)
    * [Severity](#severity)
    * [TestOrderField](#testorderfield)
    * [TestResultOrderField](#testresultorderfield)
    * [TestSuiteCrawlType](#testsuitecrawltype)
    * [TestSuiteLocationCode](#testsuitelocationcode)
    * [TestSuiteOrderField](#testsuiteorderfield)
    * [UserOrderField](#userorderfield)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [DateTime](#datetime)
    * [Float](#float)
    * [Int](#int)
    * [JSONObject](#jsonobject)
    * [ObjectID](#objectid)
    * [String](#string)

</details>

## Query
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>internalGetUser</strong></td>
<td valign="top"><a href="/#/schema?id=user">User</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetUsers</strong></td>
<td valign="top"><a href="/#/schema?id=userconnection">UserConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=userfilter">UserFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=userorder">UserOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTest</strong></td>
<td valign="top"><a href="/#/schema?id=test">Test</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTests</strong></td>
<td valign="top"><a href="/#/schema?id=testconnection">TestConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testfilter">TestFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testorder">TestOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTestSuite</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTestSuites</strong></td>
<td valign="top"><a href="/#/schema?id=testsuiteconnection">TestSuiteConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testsuitefilter">TestSuiteFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testsuiteorder">TestSuiteOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTestResult</strong></td>
<td valign="top"><a href="/#/schema?id=testresult">TestResult</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetTestResults</strong></td>
<td valign="top"><a href="/#/schema?id=testresultconnection">TestResultConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testresultfilter">TestResultFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testresultorder">TestResultOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetSegment</strong></td>
<td valign="top"><a href="/#/schema?id=segment">Segment</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetSegments</strong></td>
<td valign="top"><a href="/#/schema?id=segmentconnection">SegmentConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=segmentfilter">SegmentFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=segmentorder">SegmentOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetReport</strong></td>
<td valign="top"><a href="/#/schema?id=report">Report</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetReports</strong></td>
<td valign="top"><a href="/#/schema?id=reportconnection">ReportConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=reportfilter">ReportFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=reportorder">ReportOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetReportTemplate</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplate">ReportTemplate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetReportTemplates</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplateconnection">ReportTemplateConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=reporttemplatefilter">ReportTemplateFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=reporttemplateorder">ReportTemplateOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetProject</strong></td>
<td valign="top"><a href="/#/schema?id=project">Project</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetProjects</strong></td>
<td valign="top"><a href="/#/schema?id=projectconnection">ProjectConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=projectfilter">ProjectFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=projectorder">ProjectOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetLocation</strong></td>
<td valign="top"><a href="/#/schema?id=location">Location</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetLocations</strong></td>
<td valign="top"><a href="/#/schema?id=locationconnection">LocationConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=locationfilter">LocationFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=locationorder">LocationOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetCrawl</strong></td>
<td valign="top"><a href="/#/schema?id=crawl">Crawl</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetCrawls</strong></td>
<td valign="top"><a href="/#/schema?id=crawlconnection">CrawlConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=crawlfilter">CrawlFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=crawlorder">CrawlOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetBuild</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetBuilds</strong></td>
<td valign="top"><a href="/#/schema?id=buildconnection">BuildConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=buildfilter">BuildFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=buildorder">BuildOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetAccount</strong></td>
<td valign="top"><a href="/#/schema?id=account">Account</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalGetAccounts</strong></td>
<td valign="top"><a href="/#/schema?id=accountconnection">AccountConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=accountfilter">AccountFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=accountorder">AccountOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=entity">Entity</a></td>
<td>

Fetches an object given its ID.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=entity">Entity</a>!]!</td>
<td>

Lookup nodes by a list of IDs.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ids</td>
<td valign="top">[<a href="/#/schema?id=objectid">ObjectID</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>getTestSuiteLocations</strong></td>
<td valign="top">[<a href="/#/schema?id=location">Location</a>!]!</td>
<td>

List of locations available for test suite.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentableMetricsMetadata</strong></td>
<td valign="top">[<a href="/#/schema?id=segmentablemetricmetadata">SegmentableMetricMetadata</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>me</strong></td>
<td valign="top"><a href="/#/schema?id=user">User</a>!</td>
<td>

The currently authenticated user.

</td>
</tr>
</tbody>
</table>

## Mutation
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>abortBuild</strong></td>
<td valign="top"><a href="/#/schema?id=abortbuildpayload">AbortBuildPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=abortbuildinput">AbortBuildInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelBuild</strong></td>
<td valign="top"><a href="/#/schema?id=cancelbuildpayload">CancelBuildPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=cancelbuildinput">CancelBuildInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishBuild</strong></td>
<td valign="top"><a href="/#/schema?id=finishbuildpayload">FinishBuildPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=finishbuildinput">FinishBuildInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createBuild</strong></td>
<td valign="top"><a href="/#/schema?id=createbuildpayload">CreateBuildPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=createbuildinput">CreateBuildInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>runBuild</strong></td>
<td valign="top"><a href="/#/schema?id=runbuildpayload">RunBuildPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=runbuildinput">RunBuildInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createSegment</strong></td>
<td valign="top"><a href="/#/schema?id=createsegmentpayload">CreateSegmentPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=createsegmentinput">CreateSegmentInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteSegment</strong></td>
<td valign="top"><a href="/#/schema?id=deletesegmentpayload">DeleteSegmentPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=deletesegmentinput">DeleteSegmentInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createTestResult</strong></td>
<td valign="top"><a href="/#/schema?id=createtestresultpayload">CreateTestResultPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=createtestresultinput">CreateTestResultInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createTestSuite</strong></td>
<td valign="top"><a href="/#/schema?id=createtestsuitepayload">CreateTestSuitePayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=createtestsuiteinput">CreateTestSuiteInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateTestSuite</strong></td>
<td valign="top"><a href="/#/schema?id=updatetestsuitepayload">UpdateTestSuitePayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=updatetestsuiteinput">UpdateTestSuiteInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteTestSuite</strong></td>
<td valign="top"><a href="/#/schema?id=deletetestsuitepayload">DeleteTestSuitePayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=deletetestsuiteinput">DeleteTestSuiteInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createTest</strong></td>
<td valign="top"><a href="/#/schema?id=createtestpayload">CreateTestPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=createtestinput">CreateTestInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deleteTest</strong></td>
<td valign="top"><a href="/#/schema?id=deletetestpayload">DeleteTestPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=deletetestinput">DeleteTestInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updateTest</strong></td>
<td valign="top"><a href="/#/schema?id=updatetestpayload">UpdateTestPayload</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="/#/schema?id=updatetestinput">UpdateTestInput</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createAuthToken</strong></td>
<td valign="top"><a href="/#/schema?id=authtoken">AuthToken</a>!</td>
<td>

Generates auth token, that can be used in X-Auth-Token header.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">password</td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">username</td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createAutomatorAuthToken</strong></td>
<td valign="top"><a href="/#/schema?id=authtoken">AuthToken</a>!</td>
<td>

Generates auth token, that has 120 days expiration time.

</td>
</tr>
</tbody>
</table>

## Objects

### AbortBuildPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Account

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMax</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressCity</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressZip</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlan</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testSuites</strong></td>
<td valign="top"><a href="/#/schema?id=testsuiteconnection">TestSuiteConnection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testsuitefilter">TestSuiteFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testsuiteorder">TestSuiteOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>projects</strong></td>
<td valign="top"><a href="/#/schema?id=projectconnection">ProjectConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=projectfilter">ProjectFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=projectorder">ProjectOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>featureFlags</strong></td>
<td valign="top">[<a href="/#/schema?id=featureflag">FeatureFlag</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### AccountConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=accountedge">AccountEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=account">Account</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### AccountEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=account">Account</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### AuthToken

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Build

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ciBuildId</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passed</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawl</strong></td>
<td valign="top"><a href="/#/schema?id=crawl">Crawl</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testSuite</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="/#/schema?id=buildstatus">BuildStatus</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDcWebUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testResults</strong></td>
<td valign="top"><a href="/#/schema?id=testresultconnection">TestResultConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testresultfilter">TestResultFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testresultorder">TestResultOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### BuildConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=buildedge">BuildEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=build">Build</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### BuildEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### CancelBuildPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Crawl

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>projectId</strong> ⚠️</td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td>
<p>⚠️ <strong>DEPRECATED</strong></p>
<blockquote>

use `crawlDcWebUrl` field on Build instead of generating URL by hand

</blockquote>
</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>autoFinalize</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMax</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDisallowedPages</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNofollowLinks</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlTestSite</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettings</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAdded</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemoved</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNoindexPages</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pausedReminderSent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRewriteRules</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startedByApi</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceType</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNonHtmlFileTypes</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlExternalUrls</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNotIncludedUrls</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlability</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrend</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>incomplete</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawled</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueued</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscovered</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1At</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1At</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2At</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2At</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawled</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSteps</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmState</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractions</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupings</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isScheduled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlot</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partition</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressStepped</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevels</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessage</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteExplorer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isContainer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStats</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryEnabled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingEnabled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useEsReportStats</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlSegments</strong></td>
<td valign="top"><a href="/#/schema?id=crawlsegmentconnection">CrawlSegmentConnection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=crawlsegmentfilter">CrawlSegmentFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=crawlsegmentorder">CrawlSegmentOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reports</strong></td>
<td valign="top"><a href="/#/schema?id=reportconnection">ReportConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">segmentId</td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=reportfilter">ReportFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=reportorder">ReportOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=crawledge">CrawlEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=crawl">Crawl</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=crawl">Crawl</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### CrawlSegment

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersion</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawl</strong></td>
<td valign="top"><a href="/#/schema?id=crawl">Crawl</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segment</strong></td>
<td valign="top"><a href="/#/schema?id=segment">Segment</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlSegmentConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=crawlsegmentedge">CrawlSegmentEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=crawlsegment">CrawlSegment</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlSegmentEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=crawlsegment">CrawlSegment</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### CrawlUrl

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>amphtmlReciprocate</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>amphtml</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlIsConsistent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalizedPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatio</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetime</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlId</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>css</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionMatch</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprank</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPx</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>disallowedPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyNonIndexable</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBody</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionNonIndexable</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescription</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageNonIndexable</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleNonIndexable</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitle</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeader</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReason</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdmins</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppId</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtension</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemap</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInBacklinks</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleAnalytics</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleSearchConsole</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInList</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInLogSummary</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInSitemap</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInWebCrawl</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPage</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisits</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRate</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisits</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1Count</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1Length</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1Tag</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h2Tag</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h3Tag</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentType</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoarchive</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNofollow</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoindex</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoodp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNosnippet</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoydir</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangCombination</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnHeader</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnSitemap</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hsts</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCode</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>https</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indexable</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internal</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isImage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirectLoop</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirect</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isSelfCanonical</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>js</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>level</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktop</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobile</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotal</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharset</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentType</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaDisabledSitelinks</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoarchive</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNofollow</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoindex</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoodp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNosnippet</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoydir</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaRedirect</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifference</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentMismatch</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifference</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifference</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileReciprocate</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlIsConsistent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternate</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtml</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noarchive</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nofollowedPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noindex</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noodp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nosnippet</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noydir</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescription</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImage</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocale</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteName</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitle</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogType</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>page1</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPx</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitle</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>paginatedPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexable</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rawHeader</strong></td>
<td valign="top"><a href="/#/schema?id=jsonobject">JSONObject</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectChain</strong></td>
<td valign="top">[<a href="/#/schema?id=redirect">Redirect</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCode</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlIsConsistent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlIsConsistent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrl</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>responsive</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsNoindex</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtr</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressions</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPosition</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtr</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressions</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePosition</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtr</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressions</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPosition</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtr</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressions</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPosition</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>secureFormInputField</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateDesktop</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateMobile</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCard</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescription</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImage</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitle</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAlias</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>validTwitterCard</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>varyUserAgent</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewport</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlUrlConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=crawlurledge">CrawlUrlEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=crawlurl">CrawlUrl</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlUrlEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=crawlurl">CrawlUrl</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rawCursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateBuildPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateSegmentPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>segment</strong></td>
<td valign="top"><a href="/#/schema?id=segment">Segment</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>test</strong></td>
<td valign="top"><a href="/#/schema?id=test">Test</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestResultPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testResult</strong></td>
<td valign="top"><a href="/#/schema?id=testresult">TestResult</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestSuitePayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testSuite</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CustomDnsSetting

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>hostname</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ipAddress</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteSegmentPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>segment</strong></td>
<td valign="top"><a href="/#/schema?id=segment">Segment</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteTestPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>test</strong></td>
<td valign="top"><a href="/#/schema?id=test">Test</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteTestSuitePayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testSuite</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### FeatureFlag

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### FinishBuildPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Location

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top"><a href="/#/schema?id=locationcode">LocationCode</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enabled</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### LocationConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=locationedge">LocationEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=location">Location</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### LocationEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=location">Location</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### PageInfo

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>hasNextPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPreviousPage</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startCursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>endCursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### PredicateMetadata

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="/#/schema?id=predicate">Predicate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="/#/schema?id=primitivetype">PrimitiveType</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Project

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alertEmails</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRate</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgent</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgentShort</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSize</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSize</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirections</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidth</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatio</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAds</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalytics</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockCustom</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsString</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsUrls</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimary</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestPass</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestUser</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsExcluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsIncluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRenderer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>account</strong></td>
<td valign="top"><a href="/#/schema?id=account">Account</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawls</strong></td>
<td valign="top"><a href="/#/schema?id=crawlconnection">CrawlConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=crawlfilter">CrawlFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=crawlorder">CrawlOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segments</strong></td>
<td valign="top"><a href="/#/schema?id=segmentconnection">SegmentConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=segmentfilter">SegmentFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=segmentorder">SegmentOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### ProjectConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=projectedge">ProjectEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=project">Project</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ProjectEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=project">Project</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### ProjectUploadType

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uploadTemplate</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### Redirect

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>isMetaRedirect</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsTo</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusCode</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Report

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>change</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTime</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasChanges</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentId</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersion</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRows</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeight</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplate</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplate">ReportTemplate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawl</strong></td>
<td valign="top"><a href="/#/schema?id=crawl">Crawl</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>trend</strong></td>
<td valign="top">[<a href="/#/schema?id=report">Report</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indexName</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlUrls</strong></td>
<td valign="top"><a href="/#/schema?id=crawlurlconnection">CrawlUrlConnection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=crawlurlfilter">CrawlUrlFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=crawlurlorder">CrawlUrlOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### ReportConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=reportedge">ReportEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=report">Report</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ReportEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=report">Report</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### ReportTemplate

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>default</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isDefault</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>query</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summary</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>category</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypes</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSign</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSign</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeight</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeight</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>admin</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersion</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGrouping</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypes</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>beta</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tags</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ReportTemplateConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=reporttemplateedge">ReportTemplateEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=reporttemplate">ReportTemplate</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ReportTemplateEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplate">ReportTemplate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### RunBuildPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>build</strong></td>
<td valign="top"><a href="/#/schema?id=build">Build</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Segment

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rules</strong></td>
<td valign="top">[<a href="/#/schema?id=segmentrule">SegmentRule</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>project</strong></td>
<td valign="top"><a href="/#/schema?id=project">Project</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedBy</strong></td>
<td valign="top"><a href="/#/schema?id=user">User</a></td>
<td></td>
</tr>
</tbody>
</table>

### SegmentConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=segmentedge">SegmentEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=segment">Segment</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### SegmentEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=segment">Segment</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### SegmentRule

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metric</strong></td>
<td valign="top"><a href="/#/schema?id=segmentablemetric">SegmentableMetric</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>predicate</strong></td>
<td valign="top"><a href="/#/schema?id=predicate">Predicate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### SegmentableMetricMetadata

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="/#/schema?id=segmentablemetric">SegmentableMetric</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>predicates</strong></td>
<td valign="top">[<a href="/#/schema?id=predicatemetadata">PredicateMetadata</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### Test

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severity</strong></td>
<td valign="top"><a href="/#/schema?id=severity">Severity</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>threshold</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplate</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplate">ReportTemplate</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=testedge">TestEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=test">Test</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=test">Test</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### TestResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>passed</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severity</strong></td>
<td valign="top"><a href="/#/schema?id=severity">Severity</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplate</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplate">ReportTemplate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestResultConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=testresultedge">TestResultEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=testresult">TestResult</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestResultEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=testresult">TestResult</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### TestSuite

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alertEmails</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRate</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customDns</strong></td>
<td valign="top">[<a href="/#/schema?id=customdnssetting">CustomDnsSetting</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgent</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgentShort</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecision</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSize</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSize</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinks</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirections</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidth</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatio</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLength</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAds</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalytics</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockCustom</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsString</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsUrls</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimary</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestPass</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestUser</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsExcluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsIncluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRenderer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>account</strong></td>
<td valign="top"><a href="/#/schema?id=account">Account</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="/#/schema?id=location">Location</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tests</strong></td>
<td valign="top"><a href="/#/schema?id=testconnection">TestConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=testfilter">TestFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=testorder">TestOrder</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlTypes</strong></td>
<td valign="top">[<a href="/#/schema?id=testsuitecrawltype">TestSuiteCrawlType</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>builds</strong></td>
<td valign="top"><a href="/#/schema?id=buildconnection">BuildConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=buildfilter">BuildFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=buildorder">BuildOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=testsuiteedge">TestSuiteEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=testsuite">TestSuite</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

### UpdateTestPayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>test</strong></td>
<td valign="top"><a href="/#/schema?id=test">Test</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### UpdateTestSuitePayload

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testSuite</strong></td>
<td valign="top"><a href="/#/schema?id=testsuite">TestSuite</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### User

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>username</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>firstName</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastName</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>accounts</strong></td>
<td valign="top"><a href="/#/schema?id=accountconnection">AccountConnection</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">after</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">before</td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">filters</td>
<td valign="top">[<a href="/#/schema?id=accountfilter">AccountFilter</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top">[<a href="/#/schema?id=accountorder">AccountOrder</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### UserConnection

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>edges</strong></td>
<td valign="top">[<a href="/#/schema?id=useredge">UserEdge</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="/#/schema?id=user">User</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageInfo</strong></td>
<td valign="top"><a href="/#/schema?id=pageinfo">PageInfo</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalCount</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### UserEdge

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>node</strong></td>
<td valign="top"><a href="/#/schema?id=user">User</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cursor</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td>

Used in `before` and `after` args

</td>
</tr>
</tbody>
</table>

## Inputs

### AbortBuildInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>buildId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### AccountFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>nameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>packagePlanIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
</tbody>
</table>

### AccountOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=accountorderfield">AccountOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### BuildFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ciBuildIdIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### BuildOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=buildorderfield">BuildOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CancelBuildInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>buildId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>autoFinalizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>autoFinalizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitLevelsMaxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDisallowedPagesEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDisallowedPagesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNofollowLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNofollowLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlTestSiteEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlTestSiteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsAddedGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageSettingsRemovedGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNoindexPagesEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNoindexPagesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxProcessLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduledEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pausedReminderSentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pausedReminderSentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwriteEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwriteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRewriteRulesEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRewriteRulesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startedByApiEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startedByApiNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processInstanceTypeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNonHtmlFileTypesEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNonHtmlFileTypesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlExternalUrlsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlExternalUrlsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNotIncludedUrlsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlNotIncludedUrlsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlabilityTrendIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canceledAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transformedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>finishedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressCrawledGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>populatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveringUrlsAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>discoveredUrlsAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressEnqueuedGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressDiscoveredGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressUpdatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase1AtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase1AtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlingPhase2AtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawledPhase2AtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postTransformedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statsCrawledIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalStepLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmStateIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageGroupingsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isScheduledEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isScheduledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmExtTransitionedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fsmTransitionedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>bucketSlotGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>readyAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>archivedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>migratedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>partitionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>processedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>versionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>progressSteppedGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlLevelsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brokenAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>erroredAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>errorMessageIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scheduleRunningEmailSentAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postPopulatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteExplorerEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteExplorerNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isContainerEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isContainerNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queueingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queuedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>advancedCrawlStatsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cancelingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryEnabledEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryEnabledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingEnabledEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>refineryProcessingEnabledNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statusIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useEsReportStatsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useEsReportStatsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=crawlorderfield">CrawlOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlSegmentFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generatingAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>segmentVersionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlSegmentOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=crawlsegmentorderfield">CrawlSegmentOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CrawlUrlFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>amphtmlReciprocateEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>amphtmlReciprocateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>amphtmlEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>amphtmlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>backlinkDomainCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHeaderUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalHtmlUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalLinksInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlIsConsistentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlIsConsistentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalizedPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>canonicalizedPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentHtmlRatioGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlDatetimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlIdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cssEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cssNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction1Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction10Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction11Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction12Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction13Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction14Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction15Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction16Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction17Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction18Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction19Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction2Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction20Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction21Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction22Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction23Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction24Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction25Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction26Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction27Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction28Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction29Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction3Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction30Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction4Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction5Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction6Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction7Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction8Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Bw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Eq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Ew</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Neq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Cont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Ncont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Mreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Nmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9In</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Nin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtraction9Iemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionMatchEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customExtractionMatchNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deeprankGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthPxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>desktopUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>disallowedPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>disallowedPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyNonIndexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyNonIndexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyPrimaryUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateBodyNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionNonIndexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionNonIndexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionPrimaryUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateDescriptionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageNonIndexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageNonIndexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleNonIndexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleNonIndexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitlePrimaryUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicateTitleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encodingHeaderIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>externalLinksCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedReasonIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAdminsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fbAppIdIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fetchTimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fileExtensionIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedExternalLinksOutCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>followedLinksInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtSitemapIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundAtUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInBacklinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInBacklinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleAnalyticsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleAnalyticsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleSearchConsoleEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInGoogleSearchConsoleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInListEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInListNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInLogSummaryEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInLogSummaryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInSitemapEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInSitemapNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInWebCrawlEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundInWebCrawlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgPageLoadTimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaAvgTimeOnPageGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaPageviewsPerVisitsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitBounceRateGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gaVisitsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1CountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>h1LengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerContentTypeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoarchiveEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoarchiveNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNofollowEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNofollowNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoindexEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoindexNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoodpEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoodpNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNosnippetEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNosnippetNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoydirEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headerNoydirNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangLinksOutCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnHeaderEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnHeaderNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnSitemapEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangOnSitemapNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hreflangUrlCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hstsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>htmlSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpStatusCodeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>httpsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalLinksCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>internalNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isImageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isImageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirectLoopEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirectLoopNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirectEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isRedirectNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isSelfCanonicalEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isSelfCanonicalNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>jsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>jsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>levelGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>linksOutCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsDesktopGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsMobileGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logRequestsTotalGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaCharsetIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaContentTypeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaDisabledSitelinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaDisabledSitelinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoarchiveEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoarchiveNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNofollowEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNofollowNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoindexEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoindexNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoodpEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoodpNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNosnippetEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNosnippetNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoydirEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaNoydirNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaRedirectEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metaRedirectNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentDifferenceGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentMismatchEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopContentMismatchNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksInDifferenceGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileDesktopLinksOutDifferenceGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileReciprocateEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileReciprocateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHeaderUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateHtmlUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlIsConsistentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlIsConsistentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAlternateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobileRelAmphtmlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noarchiveEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noarchiveNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nofollowedPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nofollowedPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noindexEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noindexNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noodpEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noodpNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nosnippetEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nosnippetNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noydirEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noydirNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogDescriptionIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogImageIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogLocaleIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogSiteNameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTitleIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogTypeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ogUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>page1Eq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>page1Neq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthPxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pageTitleIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>paginatedPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>paginatedPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryPageEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryPageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNonIndexableIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToStatusCodeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectedToUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>redirectsInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relLinksInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHeaderUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextHtmlUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlIsConsistentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlIsConsistentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relNextUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHeaderUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevHtmlUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlIsConsistentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlIsConsistentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relPrevUrlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>responsiveEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>responsiveNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsNoindexEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsNoindexNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopClicksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopCtrGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopImpressionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleDesktopPositionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileClicksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileCtrGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobileImpressionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleMobilePositionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletClicksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletCtrGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletImpressionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTabletPositionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalClicksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalCtrGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalImpressionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>searchConsoleTotalPositionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>secureFormInputFieldEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>secureFormInputFieldNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateDesktopEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateDesktopNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateMobileEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>separateMobileNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitemapsInCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterCardIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterDescriptionIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterImageIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterSiteIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>twitterTitleIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlAliasIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlDigestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>validTwitterCardEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>validTwitterCardNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>varyUserAgentEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>varyUserAgentNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>viewportIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCountGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlUrlOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=crawlurlorderfield">CrawlUrlOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateBuildInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ciBuildId</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testSuiteId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateSegmentInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rules</strong></td>
<td valign="top">[<a href="/#/schema?id=createsegmentruleinput">CreateSegmentRuleInput</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>projectId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateSegmentRuleInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metric</strong></td>
<td valign="top"><a href="/#/schema?id=segmentablemetric">SegmentableMetric</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>predicate</strong></td>
<td valign="top"><a href="/#/schema?id=predicate">Predicate</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>threshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severity</strong></td>
<td valign="top"><a href="/#/schema?id=severity">Severity</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testSuiteId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestResultInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>passed</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>buildId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCode</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severity</strong></td>
<td valign="top"><a href="/#/schema?id=severity">Severity</a></td>
<td></td>
</tr>
</tbody>
</table>

### CreateTestSuiteInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>crawlTypes</strong></td>
<td valign="top">[<a href="/#/schema?id=testsuitecrawltype">TestSuiteCrawlType</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="/#/schema?id=testsuitelocationcode">TestSuiteLocationCode</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>accountId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alertEmails</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRate</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customDns</strong></td>
<td valign="top">[<a href="/#/schema?id=customdnssettinginput">CustomDnsSettingInput</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgent</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgentShort</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecision</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirections</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidth</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatio</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAds</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalytics</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockCustom</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsString</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsUrls</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimary</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestPass</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestUser</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsExcluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsIncluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRenderer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### CustomDnsSettingInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>hostname</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ipAddress</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteSegmentInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>segmentId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteTestInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### DeleteTestSuiteInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>testSuiteId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### FinishBuildInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>buildId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passed</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>failedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnedTestCount</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### LocationFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>codeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### LocationOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=locationorderfield">LocationOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ProjectFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>crawlRateEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAdsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAdsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalyticsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalyticsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRendererEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRendererNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### ProjectOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=projectorderfield">ProjectOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ReportFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generationTimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasChangesEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasChangesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTemplateCodeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypeCodeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalRowsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### ReportOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=reportorderfield">ReportOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ReportTemplateFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceCodeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>defaultEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>defaultNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isDefaultEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isDefaultNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>summaryIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>descriptionIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>categoryIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>positionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deletedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reportTypesIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalSignGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeSignGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalWeightGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changeWeightGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>adminEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>adminNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datasourceVersionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricsGroupingIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metricTypesIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>betaEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>betaNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tagsIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### ReportTemplateOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=reporttemplateorderfield">ReportTemplateOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### RunBuildInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>buildId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### SegmentFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>nameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
</tbody>
</table>

### SegmentOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=segmentorderfield">SegmentOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thresholdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### TestOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=testorderfield">TestOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestResultFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>passedEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>passedNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severityIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### TestResultOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=testresultorderfield">TestResultOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>crawlRateEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRateGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecisionGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThresholdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequestsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMaxGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequestsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSizeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinksGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTimeGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirectionsGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatioGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLengthGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAdsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAdsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalyticsEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalyticsNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsStringIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwriteIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimaryIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdEq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdNeq</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdLt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdLte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdGt</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThresholdGte</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRendererEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRendererNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwriteEq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwriteNeq</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=testsuiteorderfield">TestSuiteOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### UpdateTestInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>threshold</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>severity</strong></td>
<td valign="top"><a href="/#/schema?id=severity">Severity</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### UpdateTestSuiteInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>crawlTypes</strong></td>
<td valign="top">[<a href="/#/schema?id=testsuitecrawltype">TestSuiteCrawlType</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="/#/schema?id=testsuitelocationcode">TestSuiteLocationCode</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>testSuiteId</strong></td>
<td valign="top"><a href="/#/schema?id=objectid">ObjectID</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alertEmails</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>crawlRate</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customDns</strong></td>
<td valign="top">[<a href="/#/schema?id=customdnssettinginput">CustomDnsSettingInput</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgent</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>customHeaderUserAgentShort</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>duplicatePrecision</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emptyPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>highLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>limitPagesMax</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lowLogSummaryRequests</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxContentSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxExternalLinks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxHtmlSize</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLinks</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxLoadTime</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxRedirections</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxTitleWidth</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxUrlLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minContentRatio</strong></td>
<td valign="top"><a href="/#/schema?id=float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minDescriptionLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minTitleLength</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAds</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockAnalytics</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererBlockCustom</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsString</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rendererJsUrls</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>robotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sitePrimary</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTest</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestPass</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>siteTestUser</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thinPageThreshold</strong></td>
<td valign="top"><a href="/#/schema?id=int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsExcluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urlsIncluded</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRenderer</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useRobotsOverwrite</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

### UserFilter

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>emailBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>emailIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameBw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameEq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameEw</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameNeq</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameCont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameNcont</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameMreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameNmreg</strong></td>
<td valign="top"><a href="/#/schema?id=string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameIn</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameNin</strong></td>
<td valign="top">[<a href="/#/schema?id=string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>usernameIemp</strong></td>
<td valign="top"><a href="/#/schema?id=boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtEq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtNeq</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtLte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGt</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updatedAtGte</strong></td>
<td valign="top"><a href="/#/schema?id=datetime">DateTime</a></td>
<td></td>
</tr>
</tbody>
</table>

### UserOrder

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>field</strong></td>
<td valign="top"><a href="/#/schema?id=userorderfield">UserOrderField</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>direction</strong></td>
<td valign="top"><a href="/#/schema?id=orderdirection">OrderDirection</a>!</td>
<td></td>
</tr>
</tbody>
</table>

## Enums

### AccountOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>packagePlan</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
</tbody>
</table>

### BuildOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ciBuildId</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>finishedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>passed</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>failedTestCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>passedTestCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>warnedTestCount</strong></td>
<td></td>
</tr>
</tbody>
</table>

### BuildStatus

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Queued</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Running</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Aborted</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Cancelled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Finished</strong></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>autoFinalize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>limitLevelsMax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>limitPagesMax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlDisallowedPages</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlNofollowLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlTestSite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>languageSettings</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>languageSettingsAdded</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>languageSettingsRemoved</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlNoindexPages</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>robotsOverwrite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxProcessLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>scheduled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pausedReminderSent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useRobotsOverwrite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useRewriteRules</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>startedByApi</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>processInstanceType</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlNonHtmlFileTypes</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlExternalUrls</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlNotIncludedUrls</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlability</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlabilityTrend</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canceledAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawledAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>transformingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>transformedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>finishedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>incomplete</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>progressCrawled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>populatingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>populatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>discoveringUrlsAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>discoveredUrlsAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>progressEnqueued</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>progressDiscovered</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>progressUpdatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlingPhase1At</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawledPhase1At</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlingPhase2At</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawledPhase2At</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>postTransformingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>postTransformedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>statsCrawled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalSteps</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalStepLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fsmState</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtractions</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pageGroupings</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isScheduled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fsmExtTransitionedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fsmTransitionedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>bucketSlot</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>readyAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>archivingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>archivedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>migratingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>migratedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>partition</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>processingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>processedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>version</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>progressStepped</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlLevels</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>brokenAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>erroredAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>errorMessage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>scheduleRunningEmailSentAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>postPopulatingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>postPopulatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>siteExplorer</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isContainer</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>queueingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>queuedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>advancedCrawlStats</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>cancelingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>refineryEnabled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>refineryProcessingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>refineryProcessedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>refineryProcessingEnabled</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useEsReportStats</strong></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlSegmentOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>generatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>generatingAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>segmentVersion</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
</tbody>
</table>

### CrawlUrlOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>amphtmlReciprocate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>amphtml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>backlinkCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>backlinkDomainCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalHeaderUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalHtmlUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalLinksInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalUrlIsConsistent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>canonicalizedPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>contentHtmlRatio</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>contentSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlDatetime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlId</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>css</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction1</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction10</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction11</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction12</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction13</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction14</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction15</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction16</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction17</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction18</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction19</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction2</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction20</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction21</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction22</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction23</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction24</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction25</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction26</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction27</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction28</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction29</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction3</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction30</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction4</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction5</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction6</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction7</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction8</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtraction9</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>customExtractionMatch</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>deeprank</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>descriptionLengthPx</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>descriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>description</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>desktopUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>desktopUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>disallowedPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateBodyCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateBodyNonIndexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateBodyPrimaryUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateBodyPrimaryUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateBody</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateDescriptionCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateDescriptionNonIndexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateDescriptionPrimaryUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateDescriptionPrimaryUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateDescription</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicatePageCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicatePageNonIndexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicatePage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateTitleCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateTitleNonIndexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateTitlePrimaryUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateTitlePrimaryUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicateTitle</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>encodingHeader</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>externalLinksCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>failedReason</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fbAdmins</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fbAppId</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fetchTime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fileExtension</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>followedExternalLinksOutCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>followedLinksInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundAtSitemap</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundAtUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInBacklinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInGoogleAnalytics</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInGoogleSearchConsole</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInList</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInLogSummary</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInSitemap</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>foundInWebCrawl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>gaAvgPageLoadTime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>gaAvgTimeOnPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>gaPageviewsPerVisits</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>gaVisitBounceRate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>gaVisits</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>h1Count</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>h1Length</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>h1Tag</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>h2Tag</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>h3Tag</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerContentType</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNoarchive</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNofollow</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNoindex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNoodp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNosnippet</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>headerNoydir</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangCombination</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangLinksInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangLinksOutCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangOnHeader</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangOnPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangOnSitemap</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hreflangUrlCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hsts</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>htmlSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>httpStatusCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>https</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>indexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>internalLinksCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>internal</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isImage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isRedirectLoop</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isRedirect</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isSelfCanonical</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>js</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>level</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>linksInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>linksOutCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>logRequestsDesktop</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>logRequestsMobile</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>logRequestsTotal</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaCharset</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaContentType</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaDisabledSitelinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNoarchive</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNofollow</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNoindex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNoodp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNosnippet</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaNoydir</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metaRedirect</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileDesktopContentDifference</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileDesktopContentMismatch</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileDesktopLinksInDifference</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileDesktopLinksOutDifference</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileReciprocate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateHeaderUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateHeaderUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateHtmlUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateHtmlUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateUrlIsConsistent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternateUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAlternate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAmphtmlUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAmphtmlUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>mobileRelAmphtml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>noarchive</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>nofollowedPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>noindex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>noodp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>nosnippet</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>noydir</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogDescription</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogImage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogLocale</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogSiteName</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogTitle</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogType</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ogUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>page1</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pageTitleLengthPx</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pageTitleLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pageTitle</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paginatedPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>primaryPage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>primaryUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>primaryUrlNonIndexable</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>primaryUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>redirectCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>redirectedToStatusCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>redirectedToUrlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>redirectedToUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>redirectsInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relLinksInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relNextHeaderUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relNextHtmlUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relNextUrlIsConsistent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relNextUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relPrevHeaderUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relPrevHtmlUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relPrevUrlIsConsistent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>relPrevUrl</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>responsive</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>robotsNoindex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleDesktopClicks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleDesktopCtr</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleDesktopImpressions</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleDesktopPosition</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleMobileClicks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleMobileCtr</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleMobileImpressions</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleMobilePosition</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTabletClicks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTabletCtr</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTabletImpressions</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTabletPosition</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTotalClicks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTotalCtr</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTotalImpressions</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>searchConsoleTotalPosition</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>secureFormInputField</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>separateDesktop</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>separateMobile</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>sitemapsInCount</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterCard</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterDescriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterDescription</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterImage</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterSite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>twitterTitle</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>urlAliasDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>urlAlias</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>urlDigest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>urlLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>url</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>validTwitterCard</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>varyUserAgent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>viewport</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>wordCount</strong></td>
<td></td>
</tr>
</tbody>
</table>

### LocationCode

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Australia</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Austria</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Belgium</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Canada</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>China</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Custom</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Default</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Egypt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>France</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Germany</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Global</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>GreatBritain</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>India</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Italy</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Japan</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Netherlands</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Singapore</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Spain</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Switzerland</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Turkey</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>UnitedStates</strong></td>
<td></td>
</tr>
</tbody>
</table>

### LocationOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>code</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OrderDirection

Possible directions in which to order a list of items when provided an `orderBy` argument.

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ASC</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DESC</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Predicate

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>BeginsWith</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Contains</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>EndsWith</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Equal</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>GreaterThan</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>GreaterThanOrEqual</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>In</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>IsEmpty</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LessThan</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LessThanOrEqual</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotContain</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotEqual</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotIn</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotMatchRegex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MatchRegex</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>IsNull</strong></td>
<td></td>
</tr>
</tbody>
</table>

### PrimitiveType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>String</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Boolean</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Number</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Date</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ProjectOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlRate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>emptyPageThreshold</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>highLogSummaryRequests</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>limitPagesMax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>lowLogSummaryRequests</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxContentSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxDescriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxExternalLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxHtmlSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxLoadTime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxRedirections</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxTitleWidth</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxUrlLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minContentRatio</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minDescriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minTitleLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererBlockAds</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererBlockAnalytics</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererJsString</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>robotsOverwrite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>sitePrimary</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>siteTest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>thinPageThreshold</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useRenderer</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ReportOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>change</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>datasourceCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>generationTime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>hasChanges</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>reportTemplateCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>reportTypeCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalRows</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalWeight</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ReportTemplateOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>datasourceCode</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>default</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>isDefault</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>query</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>summary</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>description</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>category</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>position</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>deletedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>reportTypes</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalSign</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>changeSign</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>totalWeight</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>changeWeight</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>admin</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>datasourceVersion</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metricsGrouping</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>code</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>metricTypes</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>beta</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>tags</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SegmentOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>name</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
</tbody>
</table>

### SegmentableMetric

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>URL</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Severity

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Fail</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Warning</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TestOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>severity</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>threshold</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TestResultOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>passed</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>severity</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteCrawlType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Web</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>List</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteLocationCode

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Default</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Custom</strong></td>
<td></td>
</tr>
</tbody>
</table>

### TestSuiteOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>crawlRate</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>duplicatePrecision</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>emptyPageThreshold</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>highLogSummaryRequests</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>limitPagesMax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>lowLogSummaryRequests</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxContentSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxDescriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxExternalLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxHtmlSize</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxLinks</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxLoadTime</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxRedirections</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxTitleWidth</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>maxUrlLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minContentRatio</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minDescriptionLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>minTitleLength</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererBlockAds</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererBlockAnalytics</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>rendererJsString</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>robotsOverwrite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>sitePrimary</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>siteTest</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>thinPageThreshold</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useRenderer</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>useRobotsOverwrite</strong></td>
<td></td>
</tr>
</tbody>
</table>

### UserOrderField

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>id</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>username</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>createdAt</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>updatedAt</strong></td>
<td></td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

The `Boolean` scalar type represents `true` or `false`.

### DateTime

The javascript `Date` as string. Type represents date and time as the ISO Date string.

### Float

The `Float` scalar type represents signed double-precision fractional values as specified by [IEEE 754](https://en.wikipedia.org/wiki/IEEE_floating_point).

### Int

The `Int` scalar type represents non-fractional signed whole numeric values. Int can represent values between -(2^31) and 2^31 - 1.

### JSONObject

The `JSONObject` scalar type represents JSON objects as specified by [ECMA-404](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf).

### ObjectID

The ObjectID scalar type represents a unique identifier, often used to refetch an object or as key for a cache. The ObjectID type appears in a JSON response as a String; however, it is not intended to be human-readable.

### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.

