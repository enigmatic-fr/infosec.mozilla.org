---
layout: default
resource: true
categories: [Guidelines,Risk]
title: Scoring and other levels
description: Standardized scoring and other levels that aren't directly representing risk levels.
---

*The goal of this document is to ensure consistency, coherence between security documents. All Mozilla security
documentation should follow the recommendations below.*

**Note** Risk levels are not described here, but are **mandatory** when describing risk and documented in
[Standard Levels](standard_levels).

See also [Assessing Security Risk](/guidelines/assessing_security_risk) for an introduction to risk and our processes related to
risk.

## Scoring and other levels
### RFC2119 handling recommendation levels

See also [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt) for a formal
definition.

**OPTIONAL**: This is up to the reader to choose to follow or not to follow this recommendation.

**SHOULD**: Should is very close to "must do"  however, exceptions may be granted after discussion.

**MUST**: This must be done, is required, mandatory - there is no exception.

### Recommended configuration states

These are used to match recommended configuration states. It describes
set of documentation configuration state that we recommend using,
depending on your use-case.

**Modern**:
- State of the art configuration from a security point of view.
- Generally better for security sensitive services.
- Fewer server/clients may be compatible.

**Intermediate**:
- Usually the default configuration we recommend.
- Reasonable configuration that we recommend while covering the largest amount of clients.
- Fewer server/clients may be compatible, though the majority should be compatible with this configuration.

**Old**:
- Configuration that you may only use if other configurations cannot be followed for technical reasons
- Relatively safe - but must be moved to the *intermediate* configuration above when possible.
- Generally supports the largest amount of servers/clients.

### Document Status Codes

These are used in the header of every document to clearly signify its
current status.

<table>
<thead>
<tr class="header">
<th><p>Level</p></th>
<th><p>Expectations</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span class="score-green">READY</span></p></td>
<td><ul>
<li>Means the document is ready for user consumption and is expected to be followed.</li>
</ul></td>
</tr>
<tr class="even">
<td><p><span class="score-yellow">DRAFT</span></p></td>
<td><ul>
<li>Means the document is in progress or does not cover all cases.</li>
<li>You may follow this document for guidance, at your own risk.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p><span class="score-red">NOT READY</span></p></td>
<td><ul>
<li>Means the document should not be followed right now.</li>
</ul></td>
</tr>
<tr class="even">
</tr>
</tbody>
</table>

### Pass/fail tests

Tests are not levels per se. When possible, they either pass or fail.
It's similar to a walk/don't walk traffic sign.

<table>
<thead>
<tr class="header">
<th><p>Level</p></th>
<th><p>Coding rationale</p></th>
<th><p>Expectations</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span class="score-green">PASS</span></p></td>
<td><ul>
<li>Green generally means acceptance, allowance such as the traffic sign &quot;Walk&quot;.</li>
</ul></td>
<td><ul>
<li>Means a test successfully passed.</li>
<li>There is no &quot;almost passed&quot;: test must completely pass.</li>
</ul></td>
</tr>
<tr class="even">
<td><p><span class="score-red">FAIL</span></p></td>
<td><ul>
<li>Red generally means refusal, denial, such as the traffic sign &quot;Don't walk&quot;.</li>
</ul></td>
<td><ul>
<li>Means a test did not pass.</li>
</ul></td>
</tr>
<tr class="odd">
</tr>
</tbody>
</table>

### Scoring levels

Scores are used to gamify usage of security controls and features. Note
these levels do not directly signify risk, and are instead intended to
provide a grade for a particular objective. The mapping to objective can
be used as a base to create a mapping to
[Standard Levels](standard_levels).

These levels are used, for example, on the [https://observatory.mozilla.org](Mozilla Observatory).

The letter **E** is not used in the grades in order to keep scores
concise and voluntarily less granular (see expectations for each grade
below). The use of **+** and **-** modifiers is allowed if necessary.
These are added to represent going slightly above or below expectations.

<table>
<thead>
<tr class="header">
<th><p>Level</p></th>
<th><p>Expectations</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span class="score-green">A+, A, A-</span></p></td>
<td><p><em>Highest possible grade</em>.</p>
<ul>
<li>Support all features and controls.</li>
<li>All intentions of objective met.</li>
</ul></td>
</tr>
<tr class="even">
<td><p><span class="score-blue">B+, B, B-</span></p></td>
<td><ul>
<li>Supports most important features and controls.</li>
<li>Some outliers need attention.</li>
<li>Most intentions of objective met.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p><span class="score-yellow">C+, C, C-</span></p>
<p><span class="score-yellow">D+, D, D-</span></p></td>
<td><p><em>Score may moderately contribute to risk</em>.</p>
<ul>
<li>Potential service blocker.</li>
<li>Needs attention and features need to be enabled/controls added.</li>
<li>Minimal to moderate intentions of objective met.</li>
</ul></td>
</tr>
<tr class="even">
<td><p><span class="score-red">F</span></p></td>
<td><p><em>Lowest possible grade, score may greatly contribute to risk</em>.</p>
<ul>
<li>Zero to minimal intentions of objective met.</li>
<li>Immediate attention and action are required.</li>
<li>Score likely to block the service.</li>
</ul></td>
</tr>
<tr class="odd">
</tr>
</tbody>
</table>
