1. PRE-REQUIREMENTS

    1.1. Installed atlassian SDK
        https://developer.atlassian.com/display/DOCS/Set+up+the+Atlassian+Plugin+SDK+and+Build+a+Project

        Check %ATLAS_HOME%/apache-maven/bin directory is available in command line.

    1.2. Downloaded TrackDuck plugin sources

2. CONFIGURATION

    2.1. Application Link & Outgoing Authentication
        See properties in %PLUGIN_DIR%/src/main/resources/i18n-trackduck.properties

    2.2. TrackDuck button on navigation bar
        2.2.1. URL
            See section in %PLUGIN_DIR%/src/main/resources/atlassian-plugin.xml

                <web-item key="trackDuckButton"...

        2.2.2. Tooltip
            See properties in %PLUGIN_DIR%/src/main/resources/i18n-trackduck.properties

3. BUILD

    3.1. Navigate to the %PLUGIN_DIR%

    3.2. Run 'mvn clean install'

    3.3. Result: %PLUGIN_DIR%/target/jira-plugin-<version>.jar