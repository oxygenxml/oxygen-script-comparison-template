# Oxygen Script - Comparison Template
This project provides you with a template that uses <i>Oxygen Scripting Compare Directories</i> tool,
and allows you to compare two branches on your GitHub repository. It uses the most recent common ancestor 
as the base branch that the selected branches will be compared against in a 3-way comparison.

To get things ready, follow these steps:
1. Create a new GitHub project using this template. This allows you to easily create a new repository without copying and pasting the content, and with no history or reference to this repository.
   All you have to do is click the <kbd>Use this template</kbd> button. Make sure to check <i>Include all branches</i> option.
2. Get an Oxygen Scripting license key from https://www.oxygenxml.com/xml_scripting/pricing.html (you can also request a [trial](https://www.oxygenxml.com/xml_scripting/register.html)). Add it as a secret to your repository (Settings &#8594; Secrets and variables &#8594; Actions &#8594; New repository secret), and name it "SCRIPTING_LICENSE_KEY".
3. Open <i>build/gradle.properties</i> file and replace "oxygenxml" with your GitHub {userid}.

Now, as the setup should be ready, you can create or push branches to the repository, in order to compare them.
Feel free to use or remove the sample files provided with this template. To run the comparison script, follow these steps:
- In your GitHub repository, click on <b>Actions</b> tab.
- Select <b>Run Comparison Script</b> from the left panel.
- Click the <kbd>Run workflow</kbd> button in the right side.
- Type the name of the first branch to compare. 
- Type the name of the second branch to compare.
- Click <b>Run workflow</b>.

After the comparison, a report is created that provides details about the changes that were made. You can also use the SHA of commits instead of the branch names.

📝 The comparison report will be deployed to <i>gh-pages</i> branch. Make sure the workflow has read/write permissions (Settings &#8594; Actions &#8594; General &#8594; Workflow permissions). Otherwise, you may not be able to deploy your report.

The comparison report generated using Oxygen Scripting should be available here:
https://{userid}.github.io/{reponame}/comparisonReport.html

The comparison report between <i>main</i> branch of this repository and <i>test-branch</i> is available here:
https://oxygenxml.github.io/oxygen-script-comparison-template/comparisonReport.html
