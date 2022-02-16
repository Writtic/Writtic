### 👋 Hello, I'm {{ LOGIN }}

I joined GitHub on `{{ f.date(REGISTRATION_DATE, {dateStyle:"short"}) }}`.
I contributed to `{{ REPOSITORIES_CONTRIBUTED_TO }}` repositories and made `{{ COMMITS }}` commits.

<%- await include(`partials/activity.ejs`) %>

___

<%- await embed(`example-isocalendar`, {isocalendar:true, isocalendar_duration:"half-year", config_display:"large"}) %>

___

<%- await embed(`example-languages-pdf`, {lanuages:true, languages_details:"percentage, bytes-size", config_display:"large"}) %>

___

<%- await include(`partials/rss.ejs`) %>

___

<%- await embed(`example-base-pdf`, {base:"activity, community, repositories"}) %>g
