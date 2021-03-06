
# Saritasa.Web

## Import-TrustedSslCertificate

### Synopsis
Installs SSL certificate of remote server to trusted certificate root authorities store.

### Syntax
Import-TrustedSslCertificate \[-ServerHost\] &lt;String&gt; \[\[-Port\] &lt;Int32&gt;\] \[&lt;CommonParameters&gt;\]

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
			<td><nobr>ServerHost</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Port</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg">443</td>
		</tr>
	</tbody>
</table>

### Note
Based on code by Robert Westerlund and Michael J. Lyons.
http://stackoverflow.com/questions/22233702/how-to-download-the-ssl-certificate-from-a-website-using-powershell


## Update-SslCheckProcedure

### Synopsis
Disables SSL check for WebClient requests.

### Syntax
Update-SslCheckProcedure \[&lt;CommonParameters&gt;\]
