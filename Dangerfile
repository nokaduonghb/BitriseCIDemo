# ktlint check
github.dismiss_out_of_range_messages
checkstyle_format.base_path = Dir.pwd
checkstyle_format.report 'app/build/reports/ktlint/ktlintMainSourceSetCheck/ktlintMainSourceSetCheck.xml'

# android lint
android_lint.skip_gradle_task = true
android_lint.filtering = true
Dir["*/build/reports/lint-results*.xml"].each do |file|
  android_lint.report_file = file
  android_lint.lint(inline_mode: true)
end

