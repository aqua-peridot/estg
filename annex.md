# Encoded Semi-TeleGram (ESTG) - TO BE RENAMED

## Overview
ESTG encodes information in a symbolic semi-telegraphic form. Each ESTG code consists of words, numbers, and a defined symbol set. A message may map to multiple ESTG expressions; ambiguity is intrinsic. Example:  ** → “Revenue growth is approximately 10% heading into 2028.”

---

## Symbol Set

| Symbol | Function | Interpretation |
|:--------|:-----------|:----------------|
| `.` | Terminator | End of statement |
| `,` | Separator | Pause, clause division |
| `&` | Conjunction | “and” |
| `:` | Link | Label, description |
| `?` | Conditional / Uncertainty | “if”, “whether”, “maybe” |
| `~` | Approximation | “around”, “fuzzy range” |
| `%` | Probability / Fraction | Percent or ratio |
| `[]` | Group / List | Enclosed items |
| `>` | Direction / Causality / Comparison | “toward”, “causes”, “greater than” |
| `<` | Reverse Direction / Causality / Comparison | “from”, “caused by”, “less than” |
| `!` | Assertion / Exception / Warning | Strong emphasis or anomaly |

---

## Examples
<table>
  <thead>
    <tr>
      <th style="width:1em;"></th>
      <th style="width:20em;">Code</th>
      <th style="width:12em;">Meaning</th>
      <th style="width:10em;">Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>1</strong></td>
      <td>revenue growth ~2.5% > 2026.</td>
      <td>Revenue growth is expected to be around 2.5% toward 2026.</td>
      <td>Demonstrates ~ for approximation, % for fraction, > for direction.</td>
    </tr>
    <tr>
      <td><strong>2</strong></td>
      <td>Rain 5 ~ 7 days ? harvest 70% success else < 50%.</td>
      <td>If it rains for 5–7 days, harvest success is 70%; otherwise less than 50%.</td>
      <td>Uses ~ for fuzzy range, ? for conditional, % for probability, < for comparison.</td>
    </tr>
    <tr>
      <td><strong>3</strong></td>
      <td>temperature A > limit X ! , recalibrate [Y & Z] ?</td>
      <td>Temperature A exceeds limit X. Possible recalibration of Y and Z required.</td>
      <td>Applies > for greater than, ! for warning, [ ] for list, ? for uncertainty.</td>
    </tr>
    <tr>
      <td><strong>4</strong></td>
      <td>Weather ? cloudy ! . Prepare [umbrella & coat] ?</td>
      <td>Weather uncertain, possibly cloudy. Preparation with umbrella and coat advised.</td>
      <td>Employs ? for uncertainty, ! for warning, [ ] for grouping, & for conjunction.</td>
    </tr>
    <tr>
      <td><strong>5</strong></td>
      <td>Project X progress < expected ? delay risk ! . Discuss [team A & team B] > mitigation plan.</td>
      <td>Project X is behind expectations, possibly causing delay risk. Discussion with team A and B leads to mitigation planning.</td>
      <td>Uses < for lag, ? for uncertainty, ! for warning, [ ] for list, > for consequence.</td>
    </tr>
    <tr>
      <td><strong>6</strong></td>
      <td>Idea proposal ? innovative & feasible ! . Submit [draft & summary] > review.</td>
      <td>Proposal may be innovative and feasible, but caution applies. Draft and summary proceed to review.</td>
      <td>Uses ? for uncertainty, ! for caution, & for conjunction, [ ] for grouping, > for process flow.</td>
    </tr>
    <tr>
      <td><strong>7</strong></td>
      <td>Photosynthesis energy < sunlight, efficiency ~4%. Input: CO2, output: O2 > sustain life.</td>
      <td>Photosynthesis derives energy from sunlight with ~4% efficiency. CO2 intake and O2 release sustain life.</td>
      <td>Combines < for source, > for causality, and multiple clauses separated by periods.</td>
    </tr>
    <tr>
      <td><strong>8</strong></td>
      <td>Server X storage > full! . <br>Migrate options: [half > server Y: [cheaper, temp], all > cloud: durable].</td>
      <td>Server X nearing capacity. Migration options: (1) move half to server Y, cheaper and temporary; (2) move all to cloud, more durable.</td>
      <td>Uses nested [ ] for options, : for labels, > for direction or causality, ! for alert.</td>
    </tr>
    <tr>
      <td><strong>9</strong></td>
      <td>Stock $ < 90% usual ! . Consider > high risk portfolio? purchase ~1000 shares. <br> Return expected ~10% from 3%, risk high?</td>
      <td>Stock price below 90% of normal. Possible shift to high-risk portfolio and purchase of ~1000 shares. Expected return rises to ~10% from 3%, but risk likely high.</td>
      <td>Long-form example using <, !, >, ~, %, and multiple sequential clauses.</td>
    </tr>
  </tbody>
</table>

## Extended Usage: Embedded Code Snippets

ESTG codes can embed executable or pseudo-executable fragments from programming languages such as Python, Rust, or domain-specific syntaxes. Embedded code follows the same semi-telegraphic principles: minimalism, directionality, and compact causality. All embedded segments use the standardized form <code>[lang]{ ... }</code>, where <em>lang</em> is the language identifier (e.g., <code>python</code>, <code>rust</code>, <code>protoX</code>), and the inner braces contain native code without alteration.
</p>


<table>
  <thead>
    <tr>
      <th style="width:1em;"></th>
      <th style="width:22em;">Code</th>
      <th style="width:12em;">Meaning</th>
      <th style="width:10em;">Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>10</td>
      <td>Dataset size > threshold ? [python]{if x.mean() &gt; 0.5: model.fit(data)} else skip.</td>
      <td>If dataset size exceeds the threshold, execute the embedded Python code to fit the model; otherwise skip.</td>
      <td>Python code embedded inline with [python]{ ... }. ESTG maintains ? for conditional logic and > for causality.</td>
    </tr>
    <tr>
      <td>11</td>
      <td>Memory usage > 80% ! : [rust]{if usage &gt; 0.8 { alert("High memory!"); free_cache(); }}.</td>
      <td>When memory usage exceeds 80%, issue alert and free cache through embedded Rust code.</td>
      <td>Rust embedded inline with [rust]{ ... }. ! indicates warning, : introduces logic.</td>
    </tr>
    <tr>
      <td>12</td>
      <td>Process ? stable ~90% . [protoX]{task &lt;node[alpha]&gt;, retry &gt;3, delay~5s!}.</td>
      <td>Process stability around 90%. If uncertain, execute ProtoX-style command: task from node alpha, retry more than three times, delay roughly five seconds.</td>
      <td>Custom or domain-specific embedding with [protoX]{ ... }. ESTG symbols coexist with local syntax.</td>
    </tr>
    <tr>
      <td>13</td>
      <td>Temperature anomaly ? [python]{alert = temp &gt; limit; status = 'critical' if alert else 'ok'} > report.</td>
      <td>If a temperature anomaly is detected, evaluate Python snippet to assign alert flag and status, then forward report.</td>
      <td>Inline Python expression under [python]{ ... }. Preserves ? for condition and > for consequence.</td>
    </tr>
    <tr>
      <td>14</td>
      <td>Sensor reading < spec ? [rust]{let valid = false; let msg = "below spec";} ! > diagnostics.</td>
      <td>If sensor reading is below spec, embed Rust code to set validity false and message “below spec,” then raise warning and forward to diagnostics.</td>
      <td>Rust block formatted as [rust]{ ... }. ? for condition, ! for warning, > for propagation.</td>
    </tr>
  </tbody>
</table>

Presented to you by <a href="https://github.com/aqua-peridot">AP group</a>.
