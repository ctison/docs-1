---
title: Module v1
linktitle: v1
notitle: true
---

<div class="section" id="module-pulumi_kubernetes.rbac.v1">
<span id="v1"></span><h1>v1<a class="headerlink" href="#module-pulumi_kubernetes.rbac.v1" title="Permalink to this headline">¶</a></h1>
<dl class="class">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">ClusterRole</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">aggregation_rule=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">rules=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole" title="Permalink to this definition">¶</a></dt>
<dd><p>ClusterRole is a cluster level, logical grouping of PolicyRules that can be referenced as a unit
by a RoleBinding or ClusterRoleBinding.</p>
<p>Create a ClusterRole resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>aggregation_rule</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – AggregationRule is an optional field that describes how to build the Rules for this
ClusterRole. If AggregationRule is set, then the Rules are controller managed and
direct changes to Rules will be stomped by the controller.</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
<li><p><strong>rules</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Rules holds all the PolicyRules for this ClusterRole</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.aggregation_rule">
<code class="sig-name descname">aggregation_rule</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.aggregation_rule" title="Permalink to this definition">¶</a></dt>
<dd><p>AggregationRule is an optional field that describes how to build the Rules for this ClusterRole.
If AggregationRule is set, then the Rules are controller managed and direct changes to Rules
will be stomped by the controller.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.rules">
<code class="sig-name descname">rules</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.rules" title="Permalink to this definition">¶</a></dt>
<dd><p>Rules holds all the PolicyRules for this ClusterRole</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">ClusterRole</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRole.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRole.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">ClusterRoleBinding</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">role_ref=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">subjects=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>ClusterRoleBinding references a ClusterRole, but not contain it.  It can reference a ClusterRole
in the global namespace, and adds who information via Subject.</p>
<p>Create a ClusterRoleBinding resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>role_ref</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – RoleRef can only reference a ClusterRole in the global namespace. If the RoleRef
cannot be resolved, the Authorizer must return an error.</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
<li><p><strong>subjects</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Subjects holds references to the objects the role applies to.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.role_ref">
<code class="sig-name descname">role_ref</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.role_ref" title="Permalink to this definition">¶</a></dt>
<dd><p>RoleRef can only reference a ClusterRole in the global namespace. If the RoleRef cannot be
resolved, the Authorizer must return an error.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.subjects">
<code class="sig-name descname">subjects</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.subjects" title="Permalink to this definition">¶</a></dt>
<dd><p>Subjects holds references to the objects the role applies to.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">ClusterRoleBinding</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBinding.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">ClusterRoleBindingList</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">items=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList" title="Permalink to this definition">¶</a></dt>
<dd><p>ClusterRoleBindingList is a collection of ClusterRoleBindings</p>
<p>Create a ClusterRoleBindingList resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Items is a list of ClusterRoleBindings</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.items">
<code class="sig-name descname">items</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.items" title="Permalink to this definition">¶</a></dt>
<dd><p>Items is a list of ClusterRoleBindings</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">ClusterRoleBindingList</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleBindingList.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">ClusterRoleList</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">items=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList" title="Permalink to this definition">¶</a></dt>
<dd><p>ClusterRoleList is a collection of ClusterRoles</p>
<p>Create a ClusterRoleList resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Items is a list of ClusterRoles</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.items">
<code class="sig-name descname">items</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.items" title="Permalink to this definition">¶</a></dt>
<dd><p>Items is a list of ClusterRoles</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">ClusterRoleList</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.ClusterRoleList.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.ClusterRoleList.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.Role">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">Role</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">rules=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role" title="Permalink to this definition">¶</a></dt>
<dd><p>Role is a namespaced, logical grouping of PolicyRules that can be referenced as a unit by a
RoleBinding.</p>
<p>Create a Role resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
<li><p><strong>rules</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Rules holds all the PolicyRules for this Role</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.Role.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.Role.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.Role.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.Role.rules">
<code class="sig-name descname">rules</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.rules" title="Permalink to this definition">¶</a></dt>
<dd><p>Rules holds all the PolicyRules for this Role</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.Role.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">Role</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.Role.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.Role.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.Role.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">RoleBinding</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">role_ref=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">subjects=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>RoleBinding references a role, but does not contain it.  It can reference a Role in the same
namespace or a ClusterRole in the global namespace. It adds who information via Subjects and
namespace information by which namespace it exists in.  RoleBindings in a given namespace only
have effect in that namespace.</p>
<p>Create a RoleBinding resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>role_ref</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – RoleRef can reference a Role in the current namespace or a ClusterRole in the global
namespace. If the RoleRef cannot be resolved, the Authorizer must return an error.</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
<li><p><strong>subjects</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Subjects holds references to the objects the role applies to.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.role_ref">
<code class="sig-name descname">role_ref</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.role_ref" title="Permalink to this definition">¶</a></dt>
<dd><p>RoleRef can reference a Role in the current namespace or a ClusterRole in the global namespace.
If the RoleRef cannot be resolved, the Authorizer must return an error.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.subjects">
<code class="sig-name descname">subjects</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.subjects" title="Permalink to this definition">¶</a></dt>
<dd><p>Subjects holds references to the objects the role applies to.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">RoleBinding</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleBinding.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">RoleBindingList</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">items=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList" title="Permalink to this definition">¶</a></dt>
<dd><p>RoleBindingList is a collection of RoleBindings</p>
<p>Create a RoleBindingList resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Items is a list of RoleBindings</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.items">
<code class="sig-name descname">items</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.items" title="Permalink to this definition">¶</a></dt>
<dd><p>Items is a list of RoleBindings</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">RoleBindingList</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleBindingList.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleBindingList.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleList">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_kubernetes.rbac.v1.</code><code class="sig-name descname">RoleList</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">opts=None</em>, <em class="sig-param">items=None</em>, <em class="sig-param">metadata=None</em>, <em class="sig-param">__name__=None</em>, <em class="sig-param">__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList" title="Permalink to this definition">¶</a></dt>
<dd><p>RoleList is a collection of Roles</p>
<p>Create a RoleList resource with the given unique name, arguments, and options.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The <em>unique</em> name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – A bag of options that control this resource’s behavior.</p></li>
<li><p><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Items is a list of Roles</p></li>
<li><p><strong>metadata</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Standard object’s metadata.</p></li>
</ul>
</dd>
</dl>
<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.apiVersion">
<code class="sig-name descname">apiVersion</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.apiVersion" title="Permalink to this definition">¶</a></dt>
<dd><p>APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized values.
More info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#resources">https://git.k8s.io/community/contributors/devel/api-conventions.md#resources</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.kind">
<code class="sig-name descname">kind</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.kind" title="Permalink to this definition">¶</a></dt>
<dd><p>Kind is a string value representing the REST resource this object represents. Servers may infer
this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More
info: <a class="reference external" href="https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds">https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.items">
<code class="sig-name descname">items</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.items" title="Permalink to this definition">¶</a></dt>
<dd><p>Items is a list of Roles</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.metadata">
<code class="sig-name descname">metadata</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.metadata" title="Permalink to this definition">¶</a></dt>
<dd><p>Standard object’s metadata.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param">resource_name</em>, <em class="sig-param">id</em>, <em class="sig-param">opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get the state of an existing <code class="docutils literal notranslate"><span class="pre">RoleList</span></code> resource, as identified by <code class="docutils literal notranslate"><span class="pre">id</span></code>.
The ID is of the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code>; if <code class="docutils literal notranslate"><span class="pre">[namespace]</span></code> is omitted,
then (per Kubernetes convention) the ID becomes <code class="docutils literal notranslate"><span class="pre">default/[name]</span></code>.</p>
<p>Pulumi will keep track of this resource using <code class="docutils literal notranslate"><span class="pre">resource_name</span></code> as the Pulumi ID.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – <em>Unique</em> name used to register this resource with Pulumi.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An ID for the Kubernetes resource to retrieve.
Takes the form <code class="docutils literal notranslate"><span class="pre">[namespace]/[name]</span></code> or <code class="docutils literal notranslate"><span class="pre">[name]</span></code>.</p></li>
<li><p><strong>opts</strong> (<em>Optional</em><em>[</em><a class="reference internal" href="../../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a><em>]</em>) – A bag of options that control this
resource’s behavior.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="method">
<dt id="pulumi_kubernetes.rbac.v1.RoleList.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_kubernetes.rbac.v1.RoleList.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param">prop: str</em><span class="sig-paren">)</span> &#x2192; str<a class="headerlink" href="#pulumi_kubernetes.rbac.v1.RoleList.translate_input_property" title="Permalink to this definition">¶</a></dt>
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

</div>
