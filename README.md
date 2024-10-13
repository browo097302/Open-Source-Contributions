# Open-Source-Contributions
A collection of the merged open source contributions I have made, outlining the project, issue and the approach taken in solving the problem. The link to the actually PR request is found by clicking on the Issue #.

<br>

## [Splink - Fast, accurate and scalable probabilistic data linkage](https://github.com/moj-analytical-services/splink)


#### - [**Bug fix**] - Predict() Function Math Error: [Issue #2420](https://github.com/moj-analytical-services/splink/pull/2425)


**Issue**: One of the predict functions in splink was returning a math error when a threshold probability of 0 was passed in to a predict() function.

**Solution**: Traced back through the functions from where the threshold_probability was being passed in. Refactored the logic of the predict_from_comparison_vectors_sqls_using_settings function to treat threshold_match_probability as None when it is 0.

**Language**: Python

<br>

#### - [**Bug fix**] - Subtitle Error in match_weights_interactive_history_chart(): [Issue #1387](https://github.com/moj-analytical-services/splink/pull/2446)

**Issue**: The em_session.match_weights_interactive_history_chart() was returning an object id in the subtitle instead of an informative and readable string value. This is because the whole blocking rule object was being passed so it was returning an object id. 

**Solution**: Added the .blocking_rule_sql property on _blocking_rule_for_training so a readable string is returned instead of an object id code.

**Language**: Python

<br><br>

## [Project OSUS - Open Source URL Shortener](https://github.com/harshithtunuguntla/project-osus)

#### - [User Experience] - Autofocus URL input box: [Issue #26](https://github.com/harshithtunuguntla/project-osus/pull/38)

**Issue**: The cursor of the URL input field was not automatically in the url box upon the page loading

**Solution**: Added an inline JavaScript snippet at the end of the <body> tag to trigger the focus on the input field with id="longUrl". Enhances user-experience by streamlining URL shortening process.

**Language**: JavaScript


