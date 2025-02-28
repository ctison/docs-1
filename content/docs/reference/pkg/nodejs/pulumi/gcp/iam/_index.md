---
title: "Module iam"
linktitle: "iam"
meta_desc: "Explore members of the iam module in the @pulumi/gcp package."
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-google)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-gcp` repo](https://github.com/pulumi/pulumi-gcp/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-google` repo](https://github.com/terraform-providers/terraform-provider-google/issues).






<h3>Data Sources</h3>
<ul class="api">
    <li><a href="#getRule"><span class="symbol datasource"></span>getRule</a></li>
</ul>

<h3>Others</h3>
<ul class="api">
    <li><a href="#GetRuleArgs"><span class="symbol api"></span>GetRuleArgs</a></li>
    <li><a href="#GetRuleResult"><span class="symbol api"></span>GetRuleResult</a></li>
</ul>



<h2 id="data-sources">Data Sources</h2>
<h3 class="pdoc-module-header" id="getRule" data-link-title="getRule">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L23">
        Data Source <strong>getRule</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>getRule(args: <a href='#GetRuleArgs'>GetRuleArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions'>pulumi.InvokeOptions</a>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#GetRuleResult'>GetRuleResult</a>&gt; &amp; <a href='#GetRuleResult'>GetRuleResult</a></code></pre>


Use this data source to get information about a Google IAM Role.

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const roleinfo = gcp.iam.getRule({
    name: "roles/compute.viewer",
});

export const theRolePermissions = roleinfo.includedPermissions;
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/iam_role.html.markdown.


<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="GetRuleArgs" data-link-title="GetRuleArgs">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L41">
        interface <strong>GetRuleArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetRuleArgs</span></code></pre>

A collection of arguments for invoking getRule.

<h4 class="pdoc-member-header" id="GetRuleArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L45">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The name of the Role to lookup in the form `roles/{ROLE_NAME}`, `organizations/{ORGANIZATION_ID}/roles/{ROLE_NAME}` or `projects/{PROJECT_ID}/roles/{ROLE_NAME}`

<h3 class="pdoc-module-header" id="GetRuleResult" data-link-title="GetRuleResult">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L51">
        interface <strong>GetRuleResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetRuleResult</span></code></pre>

A collection of values returned by getRule.

<h4 class="pdoc-member-header" id="GetRuleResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L68">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

id is the provider-assigned unique ID for this managed resource.

<h4 class="pdoc-member-header" id="GetRuleResult-includedPermissions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L55">property <b>includedPermissions</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>includedPermissions: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];</code></pre>

specifies the list of one or more permissions to include in the custom role, such as - `iam.roles.get`

<h4 class="pdoc-member-header" id="GetRuleResult-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L56">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>
<h4 class="pdoc-member-header" id="GetRuleResult-stage">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L60">property <b>stage</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>stage: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

indicates the stage of a role in the launch lifecycle, such as `GA`, `BETA` or `ALPHA`.

<h4 class="pdoc-member-header" id="GetRuleResult-title">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/aee00383667e05eb41b74c08207661f46555a198/sdk/nodejs/iam/getRule.ts#L64">property <b>title</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>title: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

is a friendly title for the role, such as "Role Viewer"

