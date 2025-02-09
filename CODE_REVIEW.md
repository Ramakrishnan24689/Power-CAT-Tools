# Power Platform code review tool 

The Power Apps Code Review Tool is designed to streamline the evaluation of canvas apps by providing a comprehensive analysis framework. Leveraging the Power Apps Language Tooling library, this tool offers a customizable checklist of best practices, an overview of app checker results, insights into app settings, and a code/formula viewer with advanced search capabilities.

## Features
Today, the tool supports these features:

- **Customizable checklist**. The tool presents a series of patterns to examine within your application. Users can mark each pattern as pass or fail, add comments for app makers, or view additional details. Some items are automatically assessed based on detectable patterns during the initial review setup.
  
- **App Checker Integration**. Displays results from the app checker as of the app's last publication. While these results are accessible in Power Apps Studio during development, their inclusion here provides a consolidated view, helping to identify critical issues like inefficient loading or delegation problems.
  
- **App analysis**. Offers a quick assessment of essential app settings that impact performance. This section includes:
  - Screen Information: Counts the number of controls per screen to ensure it remains below the recommended maximum of 300 controls.
  - Media Files: Lists all embedded media along with their sizes.
  - Network Trace: Identifies slow network requests within the app.
    
- **Code Viewer**. Lists all screens, controls, and properties with search and filter functions, allowing users to quickly locate formulas within the app. Users can search by control name, property, or any text present in Power Apps formulas. Additionally, formulas can be linked to specific patterns, aiding in providing precise feedback to app developers.

## Creating a review

Upon launching the Power Apps Code Review Tool, you are presented with a list of existing reviews and the option to create a new one.

### Select a solution for a new review

The tool allows you to select specific solutions for evaluation. Follow these steps to initiate a review for a solution:

1. Open the Code Review Tool: Navigate to the Power Platform environment where your solution is hosted.
2. Select a Solution: From the solution list, choose the solution containing the canvas app(s) you want to review.
3. Review Setup: The tool will load all relevant apps within the selected solution. You can choose to review all or specific apps.

This selection ensures that the review process is focused and relevant to your development objectives.

### Reading a review

After selecting and reviewing a solution, the tool provides detailed analysis results.

#### Summary dashboard

The summary dashboard offers a high-level view of the review findings, including:

-  Checklist completion status: Displays the number of patterns passed, failed, or pending review.
-  App checker issues: Highlights critical warnings and errors detected during the review.
-  Performance Metrics: Provides insights into app complexity and media usage.

#### Detailed insights

- Pattern details: Each pattern includes a status indicator, comments, and links to supporting documentation.
- Code insights: View detailed formula breakdowns, search for specific control properties, and link directly to areas of concern.
- App aettings: Analyze key settings affecting app performance, such as control limits and data connections.

By reviewing these results, developers and reviewers can identify and prioritize areas for improvement, ensuring that canvas apps adhere to best practices and maintain optimal performance.

