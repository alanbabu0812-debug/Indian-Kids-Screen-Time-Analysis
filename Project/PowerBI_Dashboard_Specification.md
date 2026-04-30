# Power BI Dashboard Specification: Indian Kids Screen Time Analysis

## Data Source
- **File**: cleaned_data.csv
- **Records**: 9,714 entries
- **Age Range**: 8-18 years
- **Key Metrics**: 85.47% exceed recommended screen time limits

## Dashboard Structure (4 Pages)

### Page 1: Executive Summary & Overview
**Purpose**: High-level insights and key performance indicators

#### Key Visualizations:
1. **KPI Cards** (Top Row)
   - Total Children Surveyed: 9,714
   - Average Daily Screen Time: 4.35 hours
   - % Exceeding Recommended Limits: 85.47%
   - Most Common Health Impact: Poor Sleep

2. **Donut Chart**: Device Usage Distribution
   - Smartphone: 47.0% (4,568)
   - TV: 25.6% (2,487)
   - Laptop: 14.8% (1,433)
   - Tablet: 12.6% (1,224)

3. **Clustered Column Chart**: Screen Time by Age Group
   - X-axis: Age groups (8-10, 11-13, 14-16, 17-18)
   - Y-axis: Average screen time hours
   - Series: Gender breakdown

4. **Stacked Bar Chart**: Health Impact Distribution
   - Categories: Poor Sleep, Eye Strain, Anxiety, Obesity Risk, None
   - Show count and percentage

5. **Map Visualization**: Urban vs Rural Distribution
   - Geographic representation of screen time patterns

#### Filters & Slicers:
- Age Range Slider (8-18)
- Gender Slicer (Male/Female)
- Location Type (Urban/Rural)
- Device Type Multi-select

---

### Page 2: Device & Usage Patterns
**Purpose**: Deep dive into device preferences and usage patterns

#### Key Visualizations:
1. **Matrix Table**: Device Usage by Demographics
   - Rows: Age Groups
   - Columns: Primary Device
   - Values: Average Screen Time, Count of Users

2. **Line Chart**: Screen Time Trends by Age
   - X-axis: Age (8-18)
   - Y-axis: Average Daily Screen Time
   - Multiple lines for each device type

3. **Scatter Plot**: Educational vs Recreational Ratio
   - X-axis: Educational to Recreational Ratio
   - Y-axis: Average Screen Time
   - Size: Health Issue Count
   - Color: Device Type

4. **Waterfall Chart**: Screen Time Breakdown
   - Show how different factors contribute to total screen time

5. **Gauge Chart**: Recommended Limit Compliance
   - Show percentage within/exceeding limits
   - Color-coded (Green: Within, Red: Exceeding)

#### Advanced Analytics:
- Trend lines showing correlation between age and screen time
- Statistical measures (median, quartiles)

#### Filters & Slicers:
- Device Type (Smartphone, TV, Laptop, Tablet)
- Exceeded Recommended Limit (Yes/No)
- Educational Ratio Range Slider (0.3-0.6)

---

### Page 3: Health Impact Analysis
**Purpose**: Focus on health implications and risk factors

#### Key Visualizations:
1. **Heatmap**: Health Issues by Age and Gender
   - Rows: Age groups
   - Columns: Health impacts
   - Color intensity: Frequency of occurrence

2. **Funnel Chart**: Health Issue Severity
   - Levels: No Issues → Single Issue → Multiple Issues → Severe (3+ issues)
   - Show progression and percentages

3. **Clustered Column Chart**: Health Issues by Screen Time Ranges
   - X-axis: Screen time ranges (0-2hrs, 2-4hrs, 4-6hrs, 6+hrs)
   - Y-axis: Count of children
   - Series: Different health impacts

4. **Ribbon Chart**: Health Impact Trends by Device
   - Show how health impacts vary across different devices
   - Highlight most problematic device types

5. **Box Plot**: Screen Time Distribution by Health Impact
   - Show quartiles and outliers for each health condition

6. **Correlation Matrix**: Health Impacts Relationships
   - Show which health issues commonly occur together

#### Health Risk Indicators:
- Risk Score calculation based on multiple factors
- Color-coded alerts for high-risk groups

#### Filters & Slicers:
- Health Impact Multi-select (Poor Sleep, Eye Strain, Anxiety, Obesity Risk)
- Health Issue Count (0, 1, 2, 3, 4+)
- Screen Time Threshold Slider

---

### Page 4: Demographic & Geographic Insights
**Purpose**: Analyze patterns across different demographic segments

#### Key Visualizations:
1. **Treemap**: Population Distribution
   - Hierarchy: Location → Gender → Age Group
   - Size: Count of children
   - Color: Average screen time

2. **Stacked Area Chart**: Screen Time Evolution by Demographics
   - X-axis: Age progression
   - Y-axis: Cumulative screen time
   - Stacked by: Urban/Rural and Gender

3. **Bullet Chart**: Performance vs Targets
   - Compare actual screen time vs recommended limits
   - Broken down by demographic segments

4. **Sankey Diagram**: Flow from Demographics to Health Outcomes
   - Start: Age/Gender/Location
   - End: Health impacts
   - Show the flow and relationships

5. **Small Multiples**: Device Preference by Demographics
   - Grid of charts showing device usage patterns
   - One chart per demographic combination

6. **Comparative Bar Chart**: Urban vs Rural Analysis
   - Side-by-side comparison of key metrics
   - Screen time, device preferences, health impacts

#### Statistical Insights:
- Correlation coefficients between variables
- Significance testing results
- Confidence intervals

#### Filters & Slicers:
- Location Type (Urban/Rural)
- Age Group Multi-select
- Gender Filter
- Device Preference Filter

---

## Global Filters (Available on All Pages)

### Primary Filters:
1. **Age Range Slider**: 8-18 years (continuous)
2. **Gender Slicer**: Male, Female, All
3. **Location Slicer**: Urban, Rural, All
4. **Device Type**: Smartphone, TV, Laptop, Tablet, All
5. **Screen Time Range**: 0-14 hours (continuous slider)

### Advanced Filters:
1. **Exceeded Limit**: Yes, No, All
2. **Health Impact Presence**: Has Issues, No Issues, All
3. **Educational Ratio**: Low (0.3-0.4), Medium (0.4-0.5), High (0.5-0.6)

---

## Interactive Features

### Cross-Filtering:
- All visualizations connected for dynamic filtering
- Click on any chart element to filter other visuals
- Highlight related data points across pages

### Drill-Through:
- From summary charts to detailed breakdowns
- Age group → Individual age analysis
- Device type → Specific device insights

### Tooltips:
- Custom tooltips showing additional context
- Statistical significance indicators
- Trend information and comparisons

### Bookmarks:
- Predefined views for common analysis scenarios
- "High Risk Groups"
- "Device Comparison"
- "Age Progression Analysis"

---

## Color Scheme & Design

### Color Palette:
- **Primary**: Blue (#1f77b4) - Main data points
- **Secondary**: Orange (#ff7f0e) - Comparisons
- **Alert**: Red (#d62728) - Risk indicators
- **Success**: Green (#2ca02c) - Positive outcomes
- **Neutral**: Gray (#7f7f7f) - Background elements

### Accessibility:
- High contrast ratios
- Color-blind friendly palette
- Alternative text for all visuals
- Keyboard navigation support

---

## Performance Optimization

### Data Model:
- Star schema with fact and dimension tables
- Calculated columns for derived metrics
- Measures for dynamic calculations

### Refresh Strategy:
- Scheduled refresh if data updates regularly
- Incremental refresh for large datasets
- Data source optimization

---

## Key Insights to Highlight

1. **Critical Finding**: 85.47% of children exceed recommended screen time
2. **Device Dominance**: Smartphones account for 47% of primary device usage
3. **Health Correlation**: Strong relationship between screen time and sleep issues
4. **Age Trends**: Screen time increases with age, peaking at 16-17 years
5. **Gender Differences**: Minimal difference in average screen time between genders
6. **Urban vs Rural**: Slight difference in usage patterns (Rural: 4.37hrs vs Urban: 4.34hrs)

---

## Technical Requirements

### Power BI Features Used:
- DAX calculations for complex metrics
- Power Query for data transformation
- Custom visuals from AppSource if needed
- Row-level security for data access control

### Export Capabilities:
- PDF reports for stakeholders
- Excel export for detailed analysis
- PowerPoint integration for presentations
- Embedded analytics for web portals

This comprehensive dashboard will provide stakeholders with actionable insights into children's screen time patterns, health implications, and demographic trends, enabling data-driven decisions for digital wellness initiatives.