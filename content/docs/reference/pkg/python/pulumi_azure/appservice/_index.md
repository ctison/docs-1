---
title: Module appservice
linktitle: appservice
notitle: true
---

<div class="section" id="appservice">
<h1>appservice<a class="headerlink" href="#appservice" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div><p>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</p>
</div></blockquote>
<span class="target" id="module-pulumi_azure.appservice"></span><dl class="class">
<dt id="pulumi_azure.appservice.ActiveSlot">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">ActiveSlot</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">app_service_slot_name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot" title="Permalink to this definition">¶</a></dt>
<dd><p>Promotes an App Service Slot to Production within an App Service.</p>
<blockquote>
<div><p><strong>Note:</strong> When using Slots - the <code class="docutils literal notranslate"><span class="pre">app_settings</span></code>, <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> and <code class="docutils literal notranslate"><span class="pre">site_config</span></code> blocks on the <code class="docutils literal notranslate"><span class="pre">appservice.AppService</span></code> resource will be overwritten when promoting a Slot using the <code class="docutils literal notranslate"><span class="pre">appservice.ActiveSlot</span></code> resource.</p>
</div></blockquote>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service within which the Slot exists.  Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_service_slot_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service Slot which should be promoted to the Production Slot within the App Service.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_active_slot.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_active_slot.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.ActiveSlot.app_service_name">
<code class="sig-name descname">app_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.app_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the App Service within which the Slot exists.  Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.ActiveSlot.app_service_slot_name">
<code class="sig-name descname">app_service_slot_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.app_service_slot_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the App Service Slot which should be promoted to the Production Slot within the App Service.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.ActiveSlot.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.ActiveSlot.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">app_service_slot_name=None</em>, <em class="sig-param">resource_group_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ActiveSlot resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service within which the Slot exists.  Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_service_slot_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service Slot which should be promoted to the Production Slot within the App Service.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_active_slot.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_active_slot.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.ActiveSlot.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.ActiveSlot.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.ActiveSlot.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.AppService">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">AppService</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">backup=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">client_cert_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">logs=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">storage_accounts=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AppService" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages an App Service (within an App Service Plan).</p>
<blockquote>
<div><p><strong>Note:</strong> When using Slots - the <code class="docutils literal notranslate"><span class="pre">app_settings</span></code>, <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> and <code class="docutils literal notranslate"><span class="pre">site_config</span></code> blocks on the <code class="docutils literal notranslate"><span class="pre">appservice.AppService</span></code> resource will be overwritten when promoting a Slot using the <code class="docutils literal notranslate"><span class="pre">appservice.ActiveSlot</span></code> resource.</p>
</div></blockquote>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this App Service.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the App Service send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>client_cert_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Does the App Service require client certificates for incoming requests? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – One or more <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> blocks as defined below.</p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the App Service Enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the App Service only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A Managed Service Identity block as defined below.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>logs</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">logs</span></code> block as defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> block as defined below.</p></li>
<li><p><strong>storage_accounts</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – One or more <code class="docutils literal notranslate"><span class="pre">storage_account</span></code> blocks as defined below.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>backup</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">schedule</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">frequencyInterval</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">frequencyUnit</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">keepAtLeastOneBackup</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionPeriodInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">startTime</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">storageAccountUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>logs</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">applicationLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">level</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">httpLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">fileSystem</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInMb</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>storage_accounts</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">accessKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">accountName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">mountPath</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">shareName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.app_service_plan_id">
<code class="sig-name descname">app_service_plan_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.app_service_plan_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the App Service Plan within which to create this App Service.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.app_settings">
<code class="sig-name descname">app_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.app_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A key-value pair of App Settings.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.auth_settings">
<code class="sig-name descname">auth_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.auth_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is the App Service Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.client_affinity_enabled">
<code class="sig-name descname">client_affinity_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.client_affinity_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Should the App Service send session affinity cookies, which route client requests in the same session to the same instance?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.client_cert_enabled">
<code class="sig-name descname">client_cert_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.client_cert_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Does the App Service require client certificates for incoming requests? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.connection_strings">
<code class="sig-name descname">connection_strings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.connection_strings" title="Permalink to this definition">¶</a></dt>
<dd><p>One or more <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> blocks as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.default_site_hostname">
<code class="sig-name descname">default_site_hostname</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.default_site_hostname" title="Permalink to this definition">¶</a></dt>
<dd><p>The Default Hostname associated with the App Service - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.enabled">
<code class="sig-name descname">enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Is the App Service Enabled?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.https_only">
<code class="sig-name descname">https_only</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.https_only" title="Permalink to this definition">¶</a></dt>
<dd><p>Can the App Service only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.identity">
<code class="sig-name descname">identity</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.identity" title="Permalink to this definition">¶</a></dt>
<dd><p>A Managed Service Identity block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.logs">
<code class="sig-name descname">logs</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.logs" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">logs</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">applicationLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">level</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">httpLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">fileSystem</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInMb</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the App Service. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.outbound_ip_addresses">
<code class="sig-name descname">outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.possible_outbound_ip_addresses">
<code class="sig-name descname">possible_outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.possible_outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12,52.143.43.17</span></code> - not all of which are necessarily in use. Superset of <code class="docutils literal notranslate"><span class="pre">outbound_ip_addresses</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the App Service.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.site_config">
<code class="sig-name descname">site_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.site_config" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.site_credential">
<code class="sig-name descname">site_credential</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.site_credential" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.source_control">
<code class="sig-name descname">source_control</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.source_control" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">source_control</span></code> block as defined below, which contains the Source Control information when <code class="docutils literal notranslate"><span class="pre">scm_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">LocalGit</span></code>.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">branch</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Branch name of the Git repository for this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">repoUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - URL of the Git repository for this App Service.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.storage_accounts">
<code class="sig-name descname">storage_accounts</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.storage_accounts" title="Permalink to this definition">¶</a></dt>
<dd><p>One or more <code class="docutils literal notranslate"><span class="pre">storage_account</span></code> blocks as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">accessKey</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">accountName</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">mountPath</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">shareName</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.AppService.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.AppService.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.AppService.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">backup=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">client_cert_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">default_site_hostname=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">logs=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">outbound_ip_addresses=None</em>, <em class="sig-param">possible_outbound_ip_addresses=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">site_credential=None</em>, <em class="sig-param">source_control=None</em>, <em class="sig-param">storage_accounts=None</em>, <em class="sig-param">tags=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AppService.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing AppService resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this App Service.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the App Service send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>client_cert_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Does the App Service require client certificates for incoming requests? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – One or more <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> blocks as defined below.</p></li>
<li><p><strong>default_site_hostname</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Default Hostname associated with the App Service - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the App Service Enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the App Service only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A Managed Service Identity block as defined below.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>logs</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">logs</span></code> block as defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><strong>outbound_ip_addresses</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12</span></code></p></li>
<li><p><strong>possible_outbound_ip_addresses</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12,52.143.43.17</span></code> - not all of which are necessarily in use. Superset of <code class="docutils literal notranslate"><span class="pre">outbound_ip_addresses</span></code>.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> block as defined below.</p></li>
<li><p><strong>site_credential</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p></li>
<li><p><strong>source_control</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">source_control</span></code> block as defined below, which contains the Source Control information when <code class="docutils literal notranslate"><span class="pre">scm_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">LocalGit</span></code>.</p></li>
<li><p><strong>storage_accounts</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – One or more <code class="docutils literal notranslate"><span class="pre">storage_account</span></code> blocks as defined below.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>backup</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">schedule</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">frequencyInterval</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">frequencyUnit</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">keepAtLeastOneBackup</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionPeriodInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">startTime</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">storageAccountUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>logs</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">applicationLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">level</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">httpLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">fileSystem</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInMb</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>site_credential</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
<p>The <strong>source_control</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">branch</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Branch name of the Git repository for this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">repoUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - URL of the Git repository for this App Service.</p></li>
</ul>
<p>The <strong>storage_accounts</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">accessKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">accountName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">mountPath</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the name of the App Service. Changing this forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">shareName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.AppService.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AppService.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.AppService.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AppService.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.AwaitableGetAppServicePlanResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">AwaitableGetAppServicePlanResult</code><span class="sig-paren">(</span><em class="sig-param">is_xenon=None</em>, <em class="sig-param">kind=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">maximum_elastic_worker_count=None</em>, <em class="sig-param">maximum_number_of_workers=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">properties=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">sku=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AwaitableGetAppServicePlanResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.AwaitableGetAppServiceResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">AwaitableGetAppServiceResult</code><span class="sig-paren">(</span><em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">client_cert_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">default_site_hostname=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">outbound_ip_addresses=None</em>, <em class="sig-param">possible_outbound_ip_addresses=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_configs=None</em>, <em class="sig-param">site_credentials=None</em>, <em class="sig-param">source_controls=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AwaitableGetAppServiceResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.AwaitableGetCertificateResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">AwaitableGetCertificateResult</code><span class="sig-paren">(</span><em class="sig-param">expiration_date=None</em>, <em class="sig-param">friendly_name=None</em>, <em class="sig-param">host_names=None</em>, <em class="sig-param">issue_date=None</em>, <em class="sig-param">issuer=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">subject_name=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">thumbprint=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.AwaitableGetCertificateResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.Certificate">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">Certificate</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">key_vault_secret_id=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">password=None</em>, <em class="sig-param">pfx_blob=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Certificate" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages an App Service certificate.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>key_vault_secret_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Key Vault secret. Changing this forces a new resource to be created.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the certificate. Changing this forces a new resource to be created.</p></li>
<li><p><strong>password</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The password to access the certificate’s private key. Changing this forces a new resource to be created.</p></li>
<li><p><strong>pfx_blob</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The base64-encoded contents of the certificate. Changing this forces a new resource to be created.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the certificate. Changing this forces a new resource to be created.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_certificate.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_certificate.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.expiration_date">
<code class="sig-name descname">expiration_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.expiration_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The expiration date for the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.friendly_name">
<code class="sig-name descname">friendly_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.friendly_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The friendly name of the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.host_names">
<code class="sig-name descname">host_names</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.host_names" title="Permalink to this definition">¶</a></dt>
<dd><p>List of host names the certificate applies to.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.issue_date">
<code class="sig-name descname">issue_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.issue_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The issue date for the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.issuer">
<code class="sig-name descname">issuer</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.issuer" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the certificate issuer.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.key_vault_secret_id">
<code class="sig-name descname">key_vault_secret_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.key_vault_secret_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the Key Vault secret. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the certificate. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.password">
<code class="sig-name descname">password</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.password" title="Permalink to this definition">¶</a></dt>
<dd><p>The password to access the certificate’s private key. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.pfx_blob">
<code class="sig-name descname">pfx_blob</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.pfx_blob" title="Permalink to this definition">¶</a></dt>
<dd><p>The base64-encoded contents of the certificate. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the certificate. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.subject_name">
<code class="sig-name descname">subject_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.subject_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The subject name of the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Certificate.thumbprint">
<code class="sig-name descname">thumbprint</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Certificate.thumbprint" title="Permalink to this definition">¶</a></dt>
<dd><p>The thumbprint for the certificate.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Certificate.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">expiration_date=None</em>, <em class="sig-param">friendly_name=None</em>, <em class="sig-param">host_names=None</em>, <em class="sig-param">issue_date=None</em>, <em class="sig-param">issuer=None</em>, <em class="sig-param">key_vault_secret_id=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">password=None</em>, <em class="sig-param">pfx_blob=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">subject_name=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">thumbprint=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Certificate.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Certificate resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>expiration_date</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The expiration date for the certificate.</p></li>
<li><p><strong>friendly_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The friendly name of the certificate.</p></li>
<li><p><strong>host_names</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of host names the certificate applies to.</p></li>
<li><p><strong>issue_date</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The issue date for the certificate.</p></li>
<li><p><strong>issuer</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the certificate issuer.</p></li>
<li><p><strong>key_vault_secret_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Key Vault secret. Changing this forces a new resource to be created.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the certificate. Changing this forces a new resource to be created.</p></li>
<li><p><strong>password</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The password to access the certificate’s private key. Changing this forces a new resource to be created.</p></li>
<li><p><strong>pfx_blob</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The base64-encoded contents of the certificate. Changing this forces a new resource to be created.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the certificate. Changing this forces a new resource to be created.</p></li>
<li><p><strong>subject_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subject name of the certificate.</p></li>
<li><p><strong>thumbprint</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The thumbprint for the certificate.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_certificate.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_certificate.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Certificate.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Certificate.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Certificate.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Certificate.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.CustomHostnameBinding">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">CustomHostnameBinding</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">hostname=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">ssl_state=None</em>, <em class="sig-param">thumbprint=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages a Hostname Binding within an App Service.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service in which to add the Custom Hostname Binding. Changing this forces a new resource to be created.</p></li>
<li><p><strong>hostname</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the Custom Hostname to use for the App Service, example <code class="docutils literal notranslate"><span class="pre">www.example.com</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>ssl_state</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The SSL type. Possible values are <code class="docutils literal notranslate"><span class="pre">IpBasedEnabled</span></code> and <code class="docutils literal notranslate"><span class="pre">SniEnabled</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>thumbprint</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The SSL certificate thumbprint. Changing this forces a new resource to be created.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_custom_hostname_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_custom_hostname_binding.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.app_service_name">
<code class="sig-name descname">app_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.app_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the App Service in which to add the Custom Hostname Binding. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.hostname">
<code class="sig-name descname">hostname</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.hostname" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the Custom Hostname to use for the App Service, example <code class="docutils literal notranslate"><span class="pre">www.example.com</span></code>. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.ssl_state">
<code class="sig-name descname">ssl_state</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.ssl_state" title="Permalink to this definition">¶</a></dt>
<dd><p>The SSL type. Possible values are <code class="docutils literal notranslate"><span class="pre">IpBasedEnabled</span></code> and <code class="docutils literal notranslate"><span class="pre">SniEnabled</span></code>. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.thumbprint">
<code class="sig-name descname">thumbprint</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.thumbprint" title="Permalink to this definition">¶</a></dt>
<dd><p>The SSL certificate thumbprint. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.virtual_ip">
<code class="sig-name descname">virtual_ip</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.virtual_ip" title="Permalink to this definition">¶</a></dt>
<dd><p>The virtual IP address assigned to the hostname if IP based SSL is enabled.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">hostname=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">ssl_state=None</em>, <em class="sig-param">thumbprint=None</em>, <em class="sig-param">virtual_ip=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CustomHostnameBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service in which to add the Custom Hostname Binding. Changing this forces a new resource to be created.</p></li>
<li><p><strong>hostname</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the Custom Hostname to use for the App Service, example <code class="docutils literal notranslate"><span class="pre">www.example.com</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which the App Service exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>ssl_state</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The SSL type. Possible values are <code class="docutils literal notranslate"><span class="pre">IpBasedEnabled</span></code> and <code class="docutils literal notranslate"><span class="pre">SniEnabled</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>thumbprint</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The SSL certificate thumbprint. Changing this forces a new resource to be created.</p></li>
<li><p><strong>virtual_ip</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The virtual IP address assigned to the hostname if IP based SSL is enabled.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_custom_hostname_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_custom_hostname_binding.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.CustomHostnameBinding.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.CustomHostnameBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.FunctionApp">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">FunctionApp</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">enable_builtin_logging=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">storage_connection_string=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">version=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages a Function App.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this Function App.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the Function App send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p></li>
<li><p><strong>enable_builtin_logging</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the built-in logging of this Function App be enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the Function App enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the Function App only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the Connection String.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Function App.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p></li>
<li><p><strong>storage_connection_string</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The connection string of the backend storage account which will be used by this Function App (such as the dashboard, logs).</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
<li><p><strong>version</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The runtime version associated with the Function App. Defaults to <code class="docutils literal notranslate"><span class="pre">~1</span></code>.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the Function App enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The value for the Connection String.</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the Function App be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Linux App Framework and version for the AppService, e.g. <code class="docutils literal notranslate"><span class="pre">DOCKER|(golang:latest)</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the Function App run in 32 bit mode, rather than 64 bit mode? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Virtual Network which this App Service should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should WebSockets be enabled?</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/function_app.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/function_app.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.app_service_plan_id">
<code class="sig-name descname">app_service_plan_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.app_service_plan_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the App Service Plan within which to create this Function App.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.app_settings">
<code class="sig-name descname">app_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.app_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A key-value pair of App Settings.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.auth_settings">
<code class="sig-name descname">auth_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.auth_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is the Function App enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.client_affinity_enabled">
<code class="sig-name descname">client_affinity_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.client_affinity_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Should the Function App send session affinity cookies, which route client requests in the same session to the same instance?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.connection_strings">
<code class="sig-name descname">connection_strings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.connection_strings" title="Permalink to this definition">¶</a></dt>
<dd><p>An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The value for the Connection String.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.default_hostname">
<code class="sig-name descname">default_hostname</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.default_hostname" title="Permalink to this definition">¶</a></dt>
<dd><p>The default hostname associated with the Function App - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.enable_builtin_logging">
<code class="sig-name descname">enable_builtin_logging</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.enable_builtin_logging" title="Permalink to this definition">¶</a></dt>
<dd><p>Should the built-in logging of this Function App be enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.enabled">
<code class="sig-name descname">enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Is the Function App enabled?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.https_only">
<code class="sig-name descname">https_only</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.https_only" title="Permalink to this definition">¶</a></dt>
<dd><p>Can the Function App only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.identity">
<code class="sig-name descname">identity</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.identity" title="Permalink to this definition">¶</a></dt>
<dd><p>An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>The Function App kind - such as <code class="docutils literal notranslate"><span class="pre">functionapp,linux,container</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the Connection String.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.outbound_ip_addresses">
<code class="sig-name descname">outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.possible_outbound_ip_addresses">
<code class="sig-name descname">possible_outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.possible_outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12,52.143.43.17</span></code> - not all of which are necessarily in use. Superset of <code class="docutils literal notranslate"><span class="pre">outbound_ip_addresses</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Function App.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.site_config">
<code class="sig-name descname">site_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.site_config" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should the Function App be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Linux App Framework and version for the AppService, e.g. <code class="docutils literal notranslate"><span class="pre">DOCKER|(golang:latest)</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should the Function App run in 32 bit mode, rather than 64 bit mode? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The name of the Virtual Network which this App Service should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should WebSockets be enabled?</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.site_credential">
<code class="sig-name descname">site_credential</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.site_credential" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.storage_connection_string">
<code class="sig-name descname">storage_connection_string</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.storage_connection_string" title="Permalink to this definition">¶</a></dt>
<dd><p>The connection string of the backend storage account which will be used by this Function App (such as the dashboard, logs).</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.FunctionApp.version">
<code class="sig-name descname">version</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.version" title="Permalink to this definition">¶</a></dt>
<dd><p>The runtime version associated with the Function App. Defaults to <code class="docutils literal notranslate"><span class="pre">~1</span></code>.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.FunctionApp.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">default_hostname=None</em>, <em class="sig-param">enable_builtin_logging=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">kind=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">outbound_ip_addresses=None</em>, <em class="sig-param">possible_outbound_ip_addresses=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">site_credential=None</em>, <em class="sig-param">storage_connection_string=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">version=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing FunctionApp resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this Function App.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the Function App send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p></li>
<li><p><strong>default_hostname</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The default hostname associated with the Function App - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p></li>
<li><p><strong>enable_builtin_logging</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the built-in logging of this Function App be enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the Function App enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the Function App only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.</p></li>
<li><p><strong>kind</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Function App kind - such as <code class="docutils literal notranslate"><span class="pre">functionapp,linux,container</span></code></p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the Connection String.</p></li>
<li><p><strong>outbound_ip_addresses</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12</span></code></p></li>
<li><p><strong>possible_outbound_ip_addresses</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12,52.143.43.17</span></code> - not all of which are necessarily in use. Superset of <code class="docutils literal notranslate"><span class="pre">outbound_ip_addresses</span></code>.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Function App.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p></li>
<li><p><strong>site_credential</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p></li>
<li><p><strong>storage_connection_string</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The connection string of the backend storage account which will be used by this Function App (such as the dashboard, logs).</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
<li><p><strong>version</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The runtime version associated with the Function App. Defaults to <code class="docutils literal notranslate"><span class="pre">~1</span></code>.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the Function App enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The value for the Connection String.</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Principal ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Tenant ID for the Service Principal associated with the Managed Service Identity of this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the Function App be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Linux App Framework and version for the AppService, e.g. <code class="docutils literal notranslate"><span class="pre">DOCKER|(golang:latest)</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the Function App run in 32 bit mode, rather than 64 bit mode? Defaults to <code class="docutils literal notranslate"><span class="pre">true</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Virtual Network which this App Service should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should WebSockets be enabled?</p></li>
</ul>
<p>The <strong>site_credential</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/function_app.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/function_app.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.FunctionApp.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.FunctionApp.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.FunctionApp.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">GetAppServicePlanResult</code><span class="sig-paren">(</span><em class="sig-param">is_xenon=None</em>, <em class="sig-param">kind=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">maximum_elastic_worker_count=None</em>, <em class="sig-param">maximum_number_of_workers=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">properties=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">sku=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getAppServicePlan.</p>
<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.is_xenon">
<code class="sig-name descname">is_xenon</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.is_xenon" title="Permalink to this definition">¶</a></dt>
<dd><p>A flag that indicates if it’s a xenon plan (support for Windows Container)</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>The Operating System type of the App Service Plan</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.location" title="Permalink to this definition">¶</a></dt>
<dd><p>The Azure location where the App Service Plan exists</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.maximum_elastic_worker_count">
<code class="sig-name descname">maximum_elastic_worker_count</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.maximum_elastic_worker_count" title="Permalink to this definition">¶</a></dt>
<dd><p>The maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.maximum_number_of_workers">
<code class="sig-name descname">maximum_number_of_workers</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.maximum_number_of_workers" title="Permalink to this definition">¶</a></dt>
<dd><p>Maximum number of instances that can be assigned to this App Service plan.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.properties">
<code class="sig-name descname">properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">properties</span></code> block as documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.sku">
<code class="sig-name descname">sku</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.sku" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">sku</span></code> block as documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags assigned to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServicePlanResult.id">
<code class="sig-name descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServicePlanResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.GetAppServiceResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">GetAppServiceResult</code><span class="sig-paren">(</span><em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">client_cert_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">default_site_hostname=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">outbound_ip_addresses=None</em>, <em class="sig-param">possible_outbound_ip_addresses=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_configs=None</em>, <em class="sig-param">site_credentials=None</em>, <em class="sig-param">source_controls=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getAppService.</p>
<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.app_service_plan_id">
<code class="sig-name descname">app_service_plan_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.app_service_plan_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the App Service Plan within which the App Service exists.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.app_settings">
<code class="sig-name descname">app_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.app_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A key-value pair of App Settings for the App Service.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.client_affinity_enabled">
<code class="sig-name descname">client_affinity_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.client_affinity_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Does the App Service send session affinity cookies, which route client requests in the same session to the same instance?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.client_cert_enabled">
<code class="sig-name descname">client_cert_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.client_cert_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Does the App Service require client certificates for incoming requests?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.connection_strings">
<code class="sig-name descname">connection_strings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.connection_strings" title="Permalink to this definition">¶</a></dt>
<dd><p>An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.default_site_hostname">
<code class="sig-name descname">default_site_hostname</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.default_site_hostname" title="Permalink to this definition">¶</a></dt>
<dd><p>The Default Hostname associated with the App Service - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.enabled">
<code class="sig-name descname">enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Is the App Service Enabled?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.https_only">
<code class="sig-name descname">https_only</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.https_only" title="Permalink to this definition">¶</a></dt>
<dd><p>Can the App Service only be accessed via HTTPS?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.location" title="Permalink to this definition">¶</a></dt>
<dd><p>The Azure location where the App Service exists.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the Connection String.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.outbound_ip_addresses">
<code class="sig-name descname">outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.possible_outbound_ip_addresses">
<code class="sig-name descname">possible_outbound_ip_addresses</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.possible_outbound_ip_addresses" title="Permalink to this definition">¶</a></dt>
<dd><p>A comma separated list of outbound IP addresses - such as <code class="docutils literal notranslate"><span class="pre">52.23.25.3,52.143.43.12,52.143.43.17</span></code> - not all of which are necessarily in use. Superset of <code class="docutils literal notranslate"><span class="pre">outbound_ip_addresses</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.site_configs">
<code class="sig-name descname">site_configs</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.site_configs" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetAppServiceResult.id">
<code class="sig-name descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetAppServiceResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.GetCertificateResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">GetCertificateResult</code><span class="sig-paren">(</span><em class="sig-param">expiration_date=None</em>, <em class="sig-param">friendly_name=None</em>, <em class="sig-param">host_names=None</em>, <em class="sig-param">issue_date=None</em>, <em class="sig-param">issuer=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">subject_name=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">thumbprint=None</em>, <em class="sig-param">id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getCertificate.</p>
<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.expiration_date">
<code class="sig-name descname">expiration_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.expiration_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The expiration date for the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.friendly_name">
<code class="sig-name descname">friendly_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.friendly_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The friendly name of the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.host_names">
<code class="sig-name descname">host_names</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.host_names" title="Permalink to this definition">¶</a></dt>
<dd><p>List of host names the certificate applies to.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.issue_date">
<code class="sig-name descname">issue_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.issue_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The issue date for the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.issuer">
<code class="sig-name descname">issuer</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.issuer" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the certificate issuer.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.subject_name">
<code class="sig-name descname">subject_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.subject_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The subject name of the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.thumbprint">
<code class="sig-name descname">thumbprint</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.thumbprint" title="Permalink to this definition">¶</a></dt>
<dd><p>The thumbprint for the certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.GetCertificateResult.id">
<code class="sig-name descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.GetCertificateResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.Plan">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">Plan</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_environment_id=None</em>, <em class="sig-param">is_xenon=None</em>, <em class="sig-param">kind=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">maximum_elastic_worker_count=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">per_site_scaling=None</em>, <em class="sig-param">properties=None</em>, <em class="sig-param">reserved=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">sku=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Plan" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages an App Service Plan component.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_environment_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Environment where the App Service Plan should be located. Changing forces a new resource to be created.</p></li>
<li><p><strong>kind</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The kind of the App Service Plan to create. Possible values are <code class="docutils literal notranslate"><span class="pre">Windows</span></code> (also available as <code class="docutils literal notranslate"><span class="pre">App</span></code>), <code class="docutils literal notranslate"><span class="pre">Linux</span></code>, <code class="docutils literal notranslate"><span class="pre">elastic</span></code> (for Premium Consumption) and <code class="docutils literal notranslate"><span class="pre">FunctionApp</span></code> (for a Consumption Plan). Defaults to <code class="docutils literal notranslate"><span class="pre">Windows</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>maximum_elastic_worker_count</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the App Service Plan component. Changing this forces a new resource to be created.</p></li>
<li><p><strong>per_site_scaling</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can Apps assigned to this App Service Plan be scaled independently? If set to <code class="docutils literal notranslate"><span class="pre">false</span></code> apps assigned to this plan will scale to all instances of the plan.  Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>reserved</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is this App Service Plan <code class="docutils literal notranslate"><span class="pre">Reserved</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service Plan component.</p></li>
<li><p><strong>sku</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">sku</span></code> block as documented below.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>properties</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">app_service_environment_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The ID of the App Service Environment where the App Service Plan should be located. Changing forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">per_site_scaling</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Can Apps assigned to this App Service Plan be scaled independently? If set to <code class="docutils literal notranslate"><span class="pre">false</span></code> apps assigned to this plan will scale to all instances of the plan.  Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">reserved</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is this App Service Plan <code class="docutils literal notranslate"><span class="pre">Reserved</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
</ul>
<p>The <strong>sku</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">capacity</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>) - Specifies the number of workers associated with this App Service Plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">size</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the plan’s instance size.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tier</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the plan’s pricing tier.</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_plan.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_plan.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.app_service_environment_id">
<code class="sig-name descname">app_service_environment_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.app_service_environment_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the App Service Environment where the App Service Plan should be located. Changing forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>The kind of the App Service Plan to create. Possible values are <code class="docutils literal notranslate"><span class="pre">Windows</span></code> (also available as <code class="docutils literal notranslate"><span class="pre">App</span></code>), <code class="docutils literal notranslate"><span class="pre">Linux</span></code>, <code class="docutils literal notranslate"><span class="pre">elastic</span></code> (for Premium Consumption) and <code class="docutils literal notranslate"><span class="pre">FunctionApp</span></code> (for a Consumption Plan). Defaults to <code class="docutils literal notranslate"><span class="pre">Windows</span></code>. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.maximum_elastic_worker_count">
<code class="sig-name descname">maximum_elastic_worker_count</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.maximum_elastic_worker_count" title="Permalink to this definition">¶</a></dt>
<dd><p>The maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.maximum_number_of_workers">
<code class="sig-name descname">maximum_number_of_workers</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.maximum_number_of_workers" title="Permalink to this definition">¶</a></dt>
<dd><p>The maximum number of workers supported with the App Service Plan’s sku.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the App Service Plan component. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.per_site_scaling">
<code class="sig-name descname">per_site_scaling</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.per_site_scaling" title="Permalink to this definition">¶</a></dt>
<dd><p>Can Apps assigned to this App Service Plan be scaled independently? If set to <code class="docutils literal notranslate"><span class="pre">false</span></code> apps assigned to this plan will scale to all instances of the plan.  Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.reserved">
<code class="sig-name descname">reserved</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.reserved" title="Permalink to this definition">¶</a></dt>
<dd><p>Is this App Service Plan <code class="docutils literal notranslate"><span class="pre">Reserved</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the App Service Plan component.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.sku">
<code class="sig-name descname">sku</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.sku" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">sku</span></code> block as documented below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">capacity</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>) - Specifies the number of workers associated with this App Service Plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">size</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Specifies the plan’s instance size.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tier</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Specifies the plan’s pricing tier.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Plan.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Plan.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Plan.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_environment_id=None</em>, <em class="sig-param">is_xenon=None</em>, <em class="sig-param">kind=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">maximum_elastic_worker_count=None</em>, <em class="sig-param">maximum_number_of_workers=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">per_site_scaling=None</em>, <em class="sig-param">properties=None</em>, <em class="sig-param">reserved=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">sku=None</em>, <em class="sig-param">tags=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Plan.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Plan resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_environment_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Environment where the App Service Plan should be located. Changing forces a new resource to be created.</p></li>
<li><p><strong>kind</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The kind of the App Service Plan to create. Possible values are <code class="docutils literal notranslate"><span class="pre">Windows</span></code> (also available as <code class="docutils literal notranslate"><span class="pre">App</span></code>), <code class="docutils literal notranslate"><span class="pre">Linux</span></code>, <code class="docutils literal notranslate"><span class="pre">elastic</span></code> (for Premium Consumption) and <code class="docutils literal notranslate"><span class="pre">FunctionApp</span></code> (for a Consumption Plan). Defaults to <code class="docutils literal notranslate"><span class="pre">Windows</span></code>. Changing this forces a new resource to be created.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>maximum_elastic_worker_count</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan.</p></li>
<li><p><strong>maximum_number_of_workers</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The maximum number of workers supported with the App Service Plan’s sku.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the App Service Plan component. Changing this forces a new resource to be created.</p></li>
<li><p><strong>per_site_scaling</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can Apps assigned to this App Service Plan be scaled independently? If set to <code class="docutils literal notranslate"><span class="pre">false</span></code> apps assigned to this plan will scale to all instances of the plan.  Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>reserved</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is this App Service Plan <code class="docutils literal notranslate"><span class="pre">Reserved</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service Plan component.</p></li>
<li><p><strong>sku</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">sku</span></code> block as documented below.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>properties</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">app_service_environment_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The ID of the App Service Environment where the App Service Plan should be located. Changing forces a new resource to be created.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">per_site_scaling</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Can Apps assigned to this App Service Plan be scaled independently? If set to <code class="docutils literal notranslate"><span class="pre">false</span></code> apps assigned to this plan will scale to all instances of the plan.  Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">reserved</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is this App Service Plan <code class="docutils literal notranslate"><span class="pre">Reserved</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
</ul>
<p>The <strong>sku</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">capacity</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>) - Specifies the number of workers associated with this App Service Plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">size</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the plan’s instance size.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tier</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Specifies the plan’s pricing tier.</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_plan.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_plan.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Plan.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Plan.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Plan.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Plan.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.Slot">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">Slot</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">logs=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Slot" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages an App Service Slot (within an App Service).</p>
<blockquote>
<div><p><strong>Note:</strong> When using Slots - the <code class="docutils literal notranslate"><span class="pre">app_settings</span></code>, <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> and <code class="docutils literal notranslate"><span class="pre">site_config</span></code> blocks on the <code class="docutils literal notranslate"><span class="pre">appservice.AppService</span></code> resource will be overwritten when promoting a Slot using the <code class="docutils literal notranslate"><span class="pre">appservice.ActiveSlot</span></code> resource.</p>
</div></blockquote>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service within which to create the App Service Slot.  Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this App Service Slot. Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the App Service Slot send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the App Service Slot Enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the App Service Slot only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A Managed Service Identity block as defined below.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the Connection String.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service Slot component.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Slot Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The value for the Connection String.</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
<p>The <strong>logs</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">applicationLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">level</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">httpLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">fileSystem</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInMb</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the app be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - App command line to launch, e.g. <code class="docutils literal notranslate"><span class="pre">/sbin/myserver</span> <span class="pre">-b</span> <span class="pre">0.0.0.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>) - The ordering of default documents to load, if an address isn’t specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of the .net framework’s CLR used in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">v2.0</span></code> (which will use the latest version of the .net framework for the .net CLR v2 - currently <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">3.5</span></code>) and <code class="docutils literal notranslate"><span class="pre">v4.0</span></code> (which corresponds to the latest version of the .net CLR v4 - which at the time of writing is <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">4.7.1</span></code>). <a class="reference external" href="https://en.wikipedia.org/wiki/.NET_Framework_version_history#Overview">For more information on which .net CLR version to use based on the .net framework you’re targeting - please see this table</a>. Defaults to <code class="docutils literal notranslate"><span class="pre">v4.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is HTTP2 Enabled on this App Service? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>) - A <a class="reference external" href="https://www.terraform.io/docs/configuration/attr-as-blocks.html">List of objects</a> representing ip restrictions as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">JETTY</span></code> and <code class="docutils literal notranslate"><span class="pre">TOMCAT</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of the Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container</span></code> must also be specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of Java to use. If specified <code class="docutils literal notranslate"><span class="pre">java_container</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">1.7</span></code>, <code class="docutils literal notranslate"><span class="pre">1.8</span></code> and <code class="docutils literal notranslate"><span class="pre">11</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is “MySQL In App” Enabled? This runs a local MySQL instance with your app and shares resources from the App Service plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Managed Pipeline Mode. Possible values are <code class="docutils literal notranslate"><span class="pre">Integrated</span></code> and <code class="docutils literal notranslate"><span class="pre">Classic</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">Integrated</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The minimum supported TLS version for the app service. Possible values are <code class="docutils literal notranslate"><span class="pre">1.0</span></code>, <code class="docutils literal notranslate"><span class="pre">1.1</span></code>, and <code class="docutils literal notranslate"><span class="pre">1.2</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">1.2</span></code> for new app services.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of PHP to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">5.5</span></code>, <code class="docutils literal notranslate"><span class="pre">5.6</span></code>, <code class="docutils literal notranslate"><span class="pre">7.0</span></code>, <code class="docutils literal notranslate"><span class="pre">7.1</span></code> and <code class="docutils literal notranslate"><span class="pre">7.2</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of Python to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">2.7</span></code> and <code class="docutils literal notranslate"><span class="pre">3.4</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is Remote Debugging Enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Which version of Visual Studio should the Remote Debugger be compatible with? Possible values are <code class="docutils literal notranslate"><span class="pre">VS2012</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2013</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2015</span></code> and <code class="docutils literal notranslate"><span class="pre">VS2017</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of Source Control enabled for this App Service Slot. Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>. Possible values are: <code class="docutils literal notranslate"><span class="pre">BitbucketGit</span></code>, <code class="docutils literal notranslate"><span class="pre">BitbucketHg</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexGit</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexHg</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalHg</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code>, <code class="docutils literal notranslate"><span class="pre">LocalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">None</span></code>, <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>, <code class="docutils literal notranslate"><span class="pre">Tfs</span></code>, <code class="docutils literal notranslate"><span class="pre">VSO</span></code> and <code class="docutils literal notranslate"><span class="pre">VSTSRM</span></code></p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the App Service Slot run in 32 bit mode, rather than 64 bit mode?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Virtual Network which this App Service Slot should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should WebSockets be enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_slot.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_slot.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.app_service_name">
<code class="sig-name descname">app_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.app_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the App Service within which to create the App Service Slot.  Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.app_service_plan_id">
<code class="sig-name descname">app_service_plan_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.app_service_plan_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the App Service Plan within which to create this App Service Slot. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.app_settings">
<code class="sig-name descname">app_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.app_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A key-value pair of App Settings.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.auth_settings">
<code class="sig-name descname">auth_settings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.auth_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is the App Service Slot Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">float</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.client_affinity_enabled">
<code class="sig-name descname">client_affinity_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.client_affinity_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Should the App Service Slot send session affinity cookies, which route client requests in the same session to the same instance?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.connection_strings">
<code class="sig-name descname">connection_strings</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.connection_strings" title="Permalink to this definition">¶</a></dt>
<dd><p>An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The value for the Connection String.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.default_site_hostname">
<code class="sig-name descname">default_site_hostname</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.default_site_hostname" title="Permalink to this definition">¶</a></dt>
<dd><p>The Default Hostname associated with the App Service Slot - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.enabled">
<code class="sig-name descname">enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Is the App Service Slot Enabled?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.https_only">
<code class="sig-name descname">https_only</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.https_only" title="Permalink to this definition">¶</a></dt>
<dd><p>Can the App Service Slot only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.identity">
<code class="sig-name descname">identity</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.identity" title="Permalink to this definition">¶</a></dt>
<dd><p>A Managed Service Identity block as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.location">
<code class="sig-name descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.name">
<code class="sig-name descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the Connection String.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.resource_group_name">
<code class="sig-name descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the App Service Slot component.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.site_config">
<code class="sig-name descname">site_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.site_config" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should the app be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - App command line to launch, e.g. <code class="docutils literal notranslate"><span class="pre">/sbin/myserver</span> <span class="pre">-b</span> <span class="pre">0.0.0.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">dict</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>) - The ordering of default documents to load, if an address isn’t specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The version of the .net framework’s CLR used in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">v2.0</span></code> (which will use the latest version of the .net framework for the .net CLR v2 - currently <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">3.5</span></code>) and <code class="docutils literal notranslate"><span class="pre">v4.0</span></code> (which corresponds to the latest version of the .net CLR v4 - which at the time of writing is <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">4.7.1</span></code>). <a class="reference external" href="https://en.wikipedia.org/wiki/.NET_Framework_version_history#Overview">For more information on which .net CLR version to use based on the .net framework you’re targeting - please see this table</a>. Defaults to <code class="docutils literal notranslate"><span class="pre">v4.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is HTTP2 Enabled on this App Service? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">list</span></code>) - A <a class="reference external" href="https://www.terraform.io/docs/configuration/attr-as-blocks.html">List of objects</a> representing ip restrictions as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">JETTY</span></code> and <code class="docutils literal notranslate"><span class="pre">TOMCAT</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The version of the Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container</span></code> must also be specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The version of Java to use. If specified <code class="docutils literal notranslate"><span class="pre">java_container</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">1.7</span></code>, <code class="docutils literal notranslate"><span class="pre">1.8</span></code> and <code class="docutils literal notranslate"><span class="pre">11</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is “MySQL In App” Enabled? This runs a local MySQL instance with your app and shares resources from the App Service plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The Managed Pipeline Mode. Possible values are <code class="docutils literal notranslate"><span class="pre">Integrated</span></code> and <code class="docutils literal notranslate"><span class="pre">Classic</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">Integrated</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The minimum supported TLS version for the app service. Possible values are <code class="docutils literal notranslate"><span class="pre">1.0</span></code>, <code class="docutils literal notranslate"><span class="pre">1.1</span></code>, and <code class="docutils literal notranslate"><span class="pre">1.2</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">1.2</span></code> for new app services.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The version of PHP to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">5.5</span></code>, <code class="docutils literal notranslate"><span class="pre">5.6</span></code>, <code class="docutils literal notranslate"><span class="pre">7.0</span></code>, <code class="docutils literal notranslate"><span class="pre">7.1</span></code> and <code class="docutils literal notranslate"><span class="pre">7.2</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The version of Python to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">2.7</span></code> and <code class="docutils literal notranslate"><span class="pre">3.4</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Is Remote Debugging Enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Which version of Visual Studio should the Remote Debugger be compatible with? Possible values are <code class="docutils literal notranslate"><span class="pre">VS2012</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2013</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2015</span></code> and <code class="docutils literal notranslate"><span class="pre">VS2017</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The type of Source Control enabled for this App Service Slot. Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>. Possible values are: <code class="docutils literal notranslate"><span class="pre">BitbucketGit</span></code>, <code class="docutils literal notranslate"><span class="pre">BitbucketHg</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexGit</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexHg</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalHg</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code>, <code class="docutils literal notranslate"><span class="pre">LocalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">None</span></code>, <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>, <code class="docutils literal notranslate"><span class="pre">Tfs</span></code>, <code class="docutils literal notranslate"><span class="pre">VSO</span></code> and <code class="docutils literal notranslate"><span class="pre">VSTSRM</span></code></p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should the App Service Slot run in 32 bit mode, rather than 64 bit mode?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The name of the Virtual Network which this App Service Slot should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">bool</span></code>) - Should WebSockets be enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>)</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.site_credential">
<code class="sig-name descname">site_credential</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.site_credential" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.Slot.tags">
<code class="sig-name descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.Slot.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Slot.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">app_service_name=None</em>, <em class="sig-param">app_service_plan_id=None</em>, <em class="sig-param">app_settings=None</em>, <em class="sig-param">auth_settings=None</em>, <em class="sig-param">client_affinity_enabled=None</em>, <em class="sig-param">connection_strings=None</em>, <em class="sig-param">default_site_hostname=None</em>, <em class="sig-param">enabled=None</em>, <em class="sig-param">https_only=None</em>, <em class="sig-param">identity=None</em>, <em class="sig-param">location=None</em>, <em class="sig-param">logs=None</em>, <em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">site_config=None</em>, <em class="sig-param">site_credential=None</em>, <em class="sig-param">tags=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Slot.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Slot resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>app_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the App Service within which to create the App Service Slot.  Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_service_plan_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the App Service Plan within which to create this App Service Slot. Changing this forces a new resource to be created.</p></li>
<li><p><strong>app_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A key-value pair of App Settings.</p></li>
<li><p><strong>auth_settings</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">auth_settings</span></code> block as defined below.</p></li>
<li><p><strong>client_affinity_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Should the App Service Slot send session affinity cookies, which route client requests in the same session to the same instance?</p></li>
<li><p><strong>connection_strings</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">connection_string</span></code> block as defined below.</p></li>
<li><p><strong>default_site_hostname</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Default Hostname associated with the App Service Slot - such as <code class="docutils literal notranslate"><span class="pre">mysite.azurewebsites.net</span></code></p></li>
<li><p><strong>enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is the App Service Slot Enabled?</p></li>
<li><p><strong>https_only</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Can the App Service Slot only be accessed via HTTPS? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A Managed Service Identity block as defined below.</p></li>
<li><p><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the Connection String.</p></li>
<li><p><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the App Service Slot component.</p></li>
<li><p><strong>site_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_config</span></code> object as defined below.</p></li>
<li><p><strong>site_credential</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">site_credential</span></code> block as defined below, which contains the site-level credentials used to publish to this App Service.</p></li>
<li><p><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>auth_settings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">activeDirectory</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedAudiences</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">additionalLoginParams</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedExternalRedirectUrls</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultProvider</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is the App Service Slot Enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">facebook</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">app_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">google</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">issuer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">microsoft</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">client_id</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">client_secret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">oauthScopes</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">runtimeVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenRefreshExtensionHours</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tokenStoreEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">twitter</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerKey</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">consumerSecret</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">unauthenticatedClientAction</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>connection_strings</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">name</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Connection String.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">value</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The value for the Connection String.</p></li>
</ul>
<p>The <strong>identity</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">identityIds</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">principalId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">tenantId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">type</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of the Connection String. Possible values are <code class="docutils literal notranslate"><span class="pre">APIHub</span></code>, <code class="docutils literal notranslate"><span class="pre">Custom</span></code>, <code class="docutils literal notranslate"><span class="pre">DocDb</span></code>, <code class="docutils literal notranslate"><span class="pre">EventHub</span></code>, <code class="docutils literal notranslate"><span class="pre">MySQL</span></code>, <code class="docutils literal notranslate"><span class="pre">NotificationHub</span></code>, <code class="docutils literal notranslate"><span class="pre">PostgreSQL</span></code>, <code class="docutils literal notranslate"><span class="pre">RedisCache</span></code>, <code class="docutils literal notranslate"><span class="pre">ServiceBus</span></code>, <code class="docutils literal notranslate"><span class="pre">SQLAzure</span></code> and  <code class="docutils literal notranslate"><span class="pre">SQLServer</span></code>.</p></li>
</ul>
<p>The <strong>logs</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">applicationLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">level</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">httpLogs</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">azureBlobStorage</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">sasUrl</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">fileSystem</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>)</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInDays</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">retentionInMb</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[float]</span></code>)</p></li>
</ul>
</li>
</ul>
</li>
</ul>
<p>The <strong>site_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">alwaysOn</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the app be loaded at all times? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">appCommandLine</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - App command line to launch, e.g. <code class="docutils literal notranslate"><span class="pre">/sbin/myserver</span> <span class="pre">-b</span> <span class="pre">0.0.0.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">cors</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[dict]</span></code>) - A <code class="docutils literal notranslate"><span class="pre">cors</span></code> block as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">allowedOrigins</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">supportCredentials</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">defaultDocuments</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>) - The ordering of default documents to load, if an address isn’t specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">dotnetFrameworkVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of the .net framework’s CLR used in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">v2.0</span></code> (which will use the latest version of the .net framework for the .net CLR v2 - currently <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">3.5</span></code>) and <code class="docutils literal notranslate"><span class="pre">v4.0</span></code> (which corresponds to the latest version of the .net CLR v4 - which at the time of writing is <code class="docutils literal notranslate"><span class="pre">.net</span> <span class="pre">4.7.1</span></code>). <a class="reference external" href="https://en.wikipedia.org/wiki/.NET_Framework_version_history#Overview">For more information on which .net CLR version to use based on the .net framework you’re targeting - please see this table</a>. Defaults to <code class="docutils literal notranslate"><span class="pre">v4.0</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ftpsState</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">http2Enabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is HTTP2 Enabled on this App Service? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">ipRestrictions</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[list]</span></code>) - A <a class="reference external" href="https://www.terraform.io/docs/configuration/attr-as-blocks.html">List of objects</a> representing ip restrictions as defined below.</p>
<ul>
<li><p><code class="docutils literal notranslate"><span class="pre">ipAddress</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">subnetMask</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkSubnetId</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
</li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainer</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">JETTY</span></code> and <code class="docutils literal notranslate"><span class="pre">TOMCAT</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaContainerVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of the Java Container to use. If specified <code class="docutils literal notranslate"><span class="pre">java_version</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container</span></code> must also be specified.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">javaVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of Java to use. If specified <code class="docutils literal notranslate"><span class="pre">java_container</span></code> and <code class="docutils literal notranslate"><span class="pre">java_container_version</span></code> must also be specified. Possible values are <code class="docutils literal notranslate"><span class="pre">1.7</span></code>, <code class="docutils literal notranslate"><span class="pre">1.8</span></code> and <code class="docutils literal notranslate"><span class="pre">11</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">linuxFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">localMysqlEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is “MySQL In App” Enabled? This runs a local MySQL instance with your app and shares resources from the App Service plan.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">managedPipelineMode</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The Managed Pipeline Mode. Possible values are <code class="docutils literal notranslate"><span class="pre">Integrated</span></code> and <code class="docutils literal notranslate"><span class="pre">Classic</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">Integrated</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">minTlsVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The minimum supported TLS version for the app service. Possible values are <code class="docutils literal notranslate"><span class="pre">1.0</span></code>, <code class="docutils literal notranslate"><span class="pre">1.1</span></code>, and <code class="docutils literal notranslate"><span class="pre">1.2</span></code>. Defaults to <code class="docutils literal notranslate"><span class="pre">1.2</span></code> for new app services.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">phpVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of PHP to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">5.5</span></code>, <code class="docutils literal notranslate"><span class="pre">5.6</span></code>, <code class="docutils literal notranslate"><span class="pre">7.0</span></code>, <code class="docutils literal notranslate"><span class="pre">7.1</span></code> and <code class="docutils literal notranslate"><span class="pre">7.2</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">pythonVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The version of Python to use in this App Service Slot. Possible values are <code class="docutils literal notranslate"><span class="pre">2.7</span></code> and <code class="docutils literal notranslate"><span class="pre">3.4</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Is Remote Debugging Enabled? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">remoteDebuggingVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Which version of Visual Studio should the Remote Debugger be compatible with? Possible values are <code class="docutils literal notranslate"><span class="pre">VS2012</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2013</span></code>, <code class="docutils literal notranslate"><span class="pre">VS2015</span></code> and <code class="docutils literal notranslate"><span class="pre">VS2017</span></code>.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">scmType</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The type of Source Control enabled for this App Service Slot. Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>. Possible values are: <code class="docutils literal notranslate"><span class="pre">BitbucketGit</span></code>, <code class="docutils literal notranslate"><span class="pre">BitbucketHg</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexGit</span></code>, <code class="docutils literal notranslate"><span class="pre">CodePlexHg</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">ExternalHg</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code>, <code class="docutils literal notranslate"><span class="pre">LocalGit</span></code>, <code class="docutils literal notranslate"><span class="pre">None</span></code>, <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>, <code class="docutils literal notranslate"><span class="pre">Tfs</span></code>, <code class="docutils literal notranslate"><span class="pre">VSO</span></code> and <code class="docutils literal notranslate"><span class="pre">VSTSRM</span></code></p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">use32BitWorkerProcess</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should the App Service Slot run in 32 bit mode, rather than 64 bit mode?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">virtualNetworkName</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The name of the Virtual Network which this App Service Slot should be attached to.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">websocketsEnabled</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[bool]</span></code>) - Should WebSockets be enabled?</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">windowsFxVersion</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>)</p></li>
</ul>
<p>The <strong>site_credential</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">password</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The password associated with the username, which can be used to publish to this App Service.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">username</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The username which can be used to publish to this App Service</p></li>
</ul>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_slot.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_slot.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Slot.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Slot.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.Slot.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.Slot.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.appservice.SourceCodeToken">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">SourceCodeToken</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">token=None</em>, <em class="sig-param">token_secret=None</em>, <em class="sig-param">type=None</em>, <em class="sig-param">__props__=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages an App Service source control token.</p>
<blockquote>
<div><p><strong>NOTE:</strong> Source Control Token’s are configured at the subscription level, not on each App Service - as such this can only be configured Subscription-wide</p>
</div></blockquote>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>token</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The OAuth access token.</p></li>
<li><p><strong>token_secret</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The OAuth access token secret.</p></li>
<li><p><strong>type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The source control type. Possible values are <code class="docutils literal notranslate"><span class="pre">BitBucket</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> and <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_source_control_token.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_source_control_token.html.markdown</a>.</p>
</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.appservice.SourceCodeToken.token">
<code class="sig-name descname">token</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.token" title="Permalink to this definition">¶</a></dt>
<dd><p>The OAuth access token.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.SourceCodeToken.token_secret">
<code class="sig-name descname">token_secret</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.token_secret" title="Permalink to this definition">¶</a></dt>
<dd><p>The OAuth access token secret.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.appservice.SourceCodeToken.type">
<code class="sig-name descname">type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.type" title="Permalink to this definition">¶</a></dt>
<dd><p>The source control type. Possible values are <code class="docutils literal notranslate"><span class="pre">BitBucket</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> and <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.SourceCodeToken.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">token=None</em>, <em class="sig-param">token_secret=None</em>, <em class="sig-param">type=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SourceCodeToken resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>token</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The OAuth access token.</p></li>
<li><p><strong>token_secret</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The OAuth access token secret.</p></li>
<li><p><strong>type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The source control type. Possible values are <code class="docutils literal notranslate"><span class="pre">BitBucket</span></code>, <code class="docutils literal notranslate"><span class="pre">Dropbox</span></code>, <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> and <code class="docutils literal notranslate"><span class="pre">OneDrive</span></code>.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_source_control_token.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/app_service_source_control_token.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.SourceCodeToken.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.appservice.SourceCodeToken.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.SourceCodeToken.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="function">
<dt id="pulumi_azure.appservice.get_app_service">
<code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">get_app_service</code><span class="sig-paren">(</span><em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.get_app_service" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing App Service.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>name</strong> (<em>str</em>) – The name of the App Service.</p></li>
<li><p><strong>resource_group_name</strong> (<em>str</em>) – The Name of the Resource Group where the App Service exists.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.appservice.get_app_service_plan">
<code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">get_app_service_plan</code><span class="sig-paren">(</span><em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.get_app_service_plan" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing App Service Plan (formerly known as a <code class="docutils literal notranslate"><span class="pre">Server</span> <span class="pre">Farm</span></code>).</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>name</strong> (<em>str</em>) – The name of the App Service Plan.</p></li>
<li><p><strong>resource_group_name</strong> (<em>str</em>) – The Name of the Resource Group where the App Service Plan exists.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service_plan.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service_plan.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.appservice.get_certificate">
<code class="sig-prename descclassname">pulumi_azure.appservice.</code><code class="sig-name descname">get_certificate</code><span class="sig-paren">(</span><em class="sig-param">name=None</em>, <em class="sig-param">resource_group_name=None</em>, <em class="sig-param">tags=None</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.appservice.get_certificate" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an App Service certificate.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>name</strong> (<em>str</em>) – Specifies the name of the certificate.</p></li>
<li><p><strong>resource_group_name</strong> (<em>str</em>) – The name of the resource group in which to create the certificate.</p></li>
</ul>
</dd>
</dl>
<blockquote>
<div><p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service_certificate.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/app_service_certificate.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

</div>
