
# Saritasa.Upsource

## Get-RevisionWithoutReview

### Synopsis
Returns collection of revisions which not exists in any review with revisionId, date, author and commit message.

### Syntax
Get-RevisionWithoutReview \[-ProjectId\] &lt;String&gt; \[\[-Branch\] &lt;String&gt;\] \[\[-DaysLimit\] &lt;Int32&gt;\] \[\[-Stopwords\] &lt;String\[\]&gt;\] \[&lt;CommonParameters&gt;\]

### Parameters

<table class="table table-striped table-bordered table-condensed visible-on">
	<thead>
		<tr>
			<th>Name</th>
			<th class="visible-lg visible-md">Alias</th>
			<th>Description</th>
			<th class="visible-lg visible-md">Required?</th>
			<th class="visible-lg">Pipeline Input</th>
			<th class="visible-lg">Default Value</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><nobr>ProjectId</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Id of project, like 'crm'.</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Branch</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Branch of project, by default it's a 'develop'.</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg">develop</td>
		</tr>
		<tr>
			<td><nobr>DaysLimit</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Limit of days from 'now'.</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg">30</td>
		</tr>
		<tr>
			<td><nobr>Stopwords</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Words which will be searched in commit message and if it's include this words, that revision will be skipped.</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>

### Outputs
 - System.Object\[\]


## Initialize-Upsource

### Synopsis
Returns collection of revisions which not exists in any review with revisionId, date, author and commit message.

### Syntax
Initialize-Upsource \[-UpsourceUrl\] &lt;String&gt; \[-Credential\] &lt;PSCredential&gt; \[&lt;CommonParameters&gt;\]

### Parameters

<table class="table table-striped table-bordered table-condensed visible-on">
	<thead>
		<tr>
			<th>Name</th>
			<th class="visible-lg visible-md">Alias</th>
			<th>Description</th>
			<th class="visible-lg visible-md">Required?</th>
			<th class="visible-lg">Pipeline Input</th>
			<th class="visible-lg">Default Value</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><nobr>UpsourceUrl</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Url of the Upsource without trailing slash.</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Credential</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Credentials which will be used for Basic authentication when sending requests to Upsource.</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>
