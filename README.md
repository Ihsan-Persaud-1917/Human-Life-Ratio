# <span style="color:#C5C7C9">◈</span> Human Life Ratio <span style="color:#A64C4C">/ HLR</span>

<p align="center">
  <img src="https://placehold.co/1200x320/101114/C5C7C9?text=HUMAN+LIFE+RATIO&font=montserrat" alt="Human Life Ratio — How much of your life does it cost?" width="100%" />
</p>

<p align="center">
  <strong>How much of your life does it cost?</strong>
  <br /><br />
  <img src="https://img.shields.io/badge/STATUS-CONCEPT%20STAGE-A64C4C?style=for-the-badge" alt="Concept stage" />
  <img src="https://img.shields.io/badge/FOCUS-HUMAN--CENTRED%20ECONOMICS-C5C7C9?style=for-the-badge" alt="Human-centred economics" />
  <img src="https://img.shields.io/badge/PLATFORM-WEB-292C31?style=for-the-badge" alt="Web platform" />
</p>

<p align="center">
  <em>Economic reality, measured in human time.</em>
</p>

---

> [!IMPORTANT]
> **HLR is currently a concept-stage project.** No functioning application or validated global dataset exists yet. The methodology and features described here represent the proposed direction, not completed functionality.

## <span style="color:#C5C7C9">✳</span> The Vision

A price tells you how much money something costs. It doesn't tell you how much of your life you must spend earning it.

The same product can demand a few hours of work in one country and an entire day in another. Its monetary price tells only part of the story; the time required to afford it provides another perspective.

**Human Life Ratio (HLR)** explores a human-centred way to compare affordability across countries by measuring the working time required for a median earner to purchase a consistent basket of goods and services.

Rather than looking exclusively at prices, currencies, or economic output, HLR asks a more tangible question:

**How much working time does everyday life demand?**

## <span style="color:#A64C4C">◈</span> The Methodology

HLR is built around three stages: measuring working time, establishing an item-level benchmark, and comparing countries against it.

### 01 / Calculate working hours

For each country and item, divide the representative local retail price by the country's median hourly wage.

<p align="center">
  <strong>Working Hours Required</strong>
  <br /><br />
  <code>H[c,i] = P[c,i] / W[c]</code>
</p>

Where:

- `H[c,i]` — working hours required in country `c` to afford item `i`.
- `P[c,i]` — representative local final price of item `i`, including applicable taxes and compulsory charges where possible.
- `W[c]` — estimated median hourly wage in country `c`.

### 02 / Establish the benchmark

For each item, identify the lowest working-time requirement among all eligible countries included in the comparison.

<p align="center">
  <strong>Benchmark Hours</strong>
  <br /><br />
  <code>B[i] = min(H[c,i])</code>
</p>

This establishes the reference point for that particular item. The benchmark is not a permanent global constant; it depends on the countries and data included.

### 03 / Calculate the relative ratio

Divide each country's working-time requirement by the item's benchmark.

<p align="center">
  <strong>Item Ratio</strong>
  <br /><br />
  <code>R[c,i] = H[c,i] / B[i]</code>
</p>

The country with the lowest observed working-time requirement receives a ratio of `1.0×`. A country requiring three times as many working hours receives a ratio of `3.0×`.

### 04 / Calculate the overall HLR score

Repeat the calculation across the predefined basket of `n` eligible items, then take the arithmetic mean of the item ratios.

<p align="center">
  <strong>Human Life Ratio</strong>
  <br /><br />
  <code>HLR[c] = (1 / n) × Σ R[c,i]</code>
  <br /><br />
  <sub>Sum the item's relative ratios for country c, then divide by the number of included items.</sub>
</p>

### An illustrative example

| Country | Hours required | Item ratio |
|:--|--:|--:|
| Country A | 2 | 1.0× |
| Country B | 6 | 3.0× |
| Country C | 10 | 5.0× |

Country A establishes the benchmark. Country C requires five times as many working hours to afford the same item.

<sub>Illustrative figures only. They do not represent real countries or observed data.</sub>

## <span style="color:#C5C7C9">⌘</span> What It Could Become

<table>
  <tr>
    <td width="50%">
      <h3><span style="color:#C5C7C9">◉</span> Global Explorer</h3>
      Explore an interactive globe, inspect country scores, and navigate from a global view to individual profiles.
    </td>
    <td width="50%">
      <h3><span style="color:#C5C7C9">≡</span> Rankings & Comparisons</h3>
      Explore overall rankings, compare up to seven countries, and investigate how individual items affect their results.
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3><span style="color:#A64C4C">◇</span> Scenario Sandbox</h3>
      Adjust hypothetical wages, prices, and assumptions to explore alternative scenarios without confusing them with published observations.
    </td>
    <td width="50%">
      <h3><span style="color:#748B83">↗</span> Transparent Data</h3>
      Inspect sources and data coverage, submit corrections, and eventually contribute observations for review.
    </td>
  </tr>
</table>

The initial basket is expected to contain approximately **20–30 representative goods and services**, potentially spanning food, housing, transport, technology, education, and healthcare.

<sub>These are proposed features and categories. Final scope and item selection remain undecided.</sub>

## <span style="color:#748B83">◎</span> Design Philosophy

HLR should feel like a precision instrument for exploring economic reality—not another generic fintech dashboard.

| Principle | Direction |
|:--|:--|
| <span style="color:#C5C7C9">**Human-centred**</span> | Express affordability in working time people can relate to. |
| <span style="color:#C5C7C9">**Transparent**</span> | Keep formulas, assumptions, sources, and limitations accessible. |
| <span style="color:#C5C7C9">**Evidence-led**</span> | Distinguish observed data from estimates and hypothetical scenarios. |
| <span style="color:#C5C7C9">**Precisely engineered**</span> | Use clear hierarchy, consistent comparisons, and deliberate geometry. |

### Visual identity / Obsidian & Titanium

<table>
  <tr>
    <td align="center" width="25%">
      <img src="https://placehold.co/120x64/101114/101114.png" alt="Obsidian black" width="100%" />
      <strong>Obsidian</strong><br /><code>#101114</code>
    </td>
    <td align="center" width="25%">
      <img src="https://placehold.co/120x64/C5C7C9/C5C7C9.png" alt="Titanium" width="100%" />
      <strong>Titanium</strong><br /><code>#C5C7C9</code>
    </td>
    <td align="center" width="25%">
      <img src="https://placehold.co/120x64/A64C4C/A64C4C.png" alt="Oxide red" width="100%" />
      <strong>Oxide Red</strong><br /><code>#A64C4C</code>
    </td>
    <td align="center" width="25%">
      <img src="https://placehold.co/120x64/748B83/748B83.png" alt="Muted silver-green" width="100%" />
      <strong>Silver-Green</strong><br /><code>#748B83</code>
    </td>
  </tr>
</table>

Sharp rectangular geometry, fine titanium borders, restrained oxide-red accents, and generous negative space define the visual direction. Glass and translucency should be used selectively, while typography and data remain the focus.

**No unnecessary pills. No decorative clutter. Just structure, contrast, and precision.**

## <span style="color:#A64C4C">!</span> Important Considerations & Disclaimer

HLR is an exploratory affordability indicator, not a proven replacement for GDP, purchasing power parity, cost-of-living indices, or broader measures of human development.

Its usefulness will depend on methodological consistency and data quality:

- **Wage comparability:** Median hourly wages must be defined consistently. Annual salaries require appropriate assumptions about working hours rather than an arbitrary universal conversion.
- **Price comparability:** Products and services need consistent specifications, representative local prices, and documented tax treatment.
- **Coverage:** Missing or unreliable observations must not be treated as zero or assigned the best ratio. Comparisons must disclose their coverage.
- **Benchmark dependence:** Item ratios can change when the best-performing country or the eligible comparison group changes.
- **Local context:** Public services, subsidies, informal work, unemployment, inequality, and differences in product quality can substantially affect lived affordability.
- **Interpretation:** An average of relative item ratios is not a literal measure of total living costs, personal welfare, or quality of life.

Prices and wages will be compared in the same local currency, so currency conversion is not required for the working-hours calculation itself. However, exchange rates can still influence local prices, particularly for imported goods.

**HLR aims to complement existing economic measures by examining affordability through working time. Its conclusions must remain proportionate to the evidence and assumptions behind them.**

## <span style="color:#C5C7C9">⌘</span> The Road Ahead

<details>
<summary><strong>01 — Foundations</strong></summary>

- [ ] Define the initial methodology and item basket.
- [ ] Establish data, benchmark, and missing-value rules.
- [ ] Prototype and validate the calculation engine.

</details>

<details>
<summary><strong>02 — Exploration</strong></summary>

- [ ] Build the interactive globe and country profiles.
- [ ] Introduce rankings and country comparisons.
- [ ] Display source data and coverage alongside results.

</details>

<details>
<summary><strong>03 — Expansion</strong></summary>

- [ ] Develop the scenario sandbox and reviewed data contributions.
- [ ] Explore historical tracking and broader data coverage.
- [ ] Evaluate reliability and comparability across countries.

</details>

<sub>Exploratory milestones, not delivery commitments.</sub>

## <span style="color:#C5C7C9">◇</span> Project Status

| Attribute | Current direction |
|:--|:--|
| **Project** | Human Life Ratio (HLR) |
| **Stage** | Concept / pre-implementation |
| **Focus** | Comparative affordability measured in working time |
| **Platform** | Interactive web experience |
| **Initial basket** | Approximately 20–30 proposed items |
| **Technology stack** | Undecided |
| **License** | Undecided |

---

<p align="center">
  <br />
  <strong><span style="color:#C5C7C9">HUMAN LIFE RATIO</span> <span style="color:#A64C4C">/ HLR</span></strong>
  <br />
  <em>How much of your life does it cost?</em>
  <br /><br />
  <sub>An idea at the beginning of its journey.</sub>
</p>
