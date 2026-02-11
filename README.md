# RUBY SECURITY PROJECTS and VULNERABLE REPOs

---
## @jasnow TODO

 * Get "Security on Rails" code URL. (2/10/2026: Not in ESN or Github)
   * 2/10/2026
     a. https://github.com/pragmaticprogrammer/security-on-rails (not found)
     b. Download purchased book PDF from publisher. (done)

 * Learn more about:
   * https://github.com/jasnow/ruby-goof
   * https://github.com/jasnow/vulnerable-rails-contrast
   * https://guides.rubyonrails.org/security.html

 * Auto run the security tool against vulnerable repos.

---
## Ruby Security Project Ideas (as of 2/11/2026)

 1. Rewrite [ruby-advisory-db](https://github.com/rubysec/ruby-advisory-db])/lib/github_advisory_sync.rb ruby script.
    This project is used by "bundle audit" command.

 2. Add more vulnerabilities to [Railsgoat](https://github.com/jasnow/railsgoat) Training repo/project.
    * Compare Railsgoat vs. above 2 security books.

 3. Support [ruby_audit](https://github.com/civisanalytics/ruby_audit) project.

---

 5. Modernize 2xxx "Black Hat Ruby" book's [code](https://github.com/blackhatruby/BHR_Labs]).

 6. Modernize 2009 [Security on Rails](https://www.oreilly.com/pub/pr/2486) book's code. Add URL.
    * URL: ???

---
## PAST Ruby/Rails GSOC Involvement
    * Ruby:    2016,2018-2023
    * Rails:   2017-2018
    * sciruby: 2016-2019

    * 2026
      * https://github.com/rubygsoc/rubygsoc/wiki/Ideas-List-(2026)
    * 2020
      * https://groups.google.com/g/sciruby-dev/c/AA4n4URIAE0
    * 2017
      * https://rubyonrails.org/2017/3/2/google-summer-of-code-2017
        * https://github.com/railsgsoc/ideas/wiki/2017-Ideas
    * 2016
      * https://github.com/railsgsoc/ideas/wiki/2016-Ideas
      * https://github.com/jruby/jruby/wiki/Google-Summer-of-Code-2016
    * 2015
      * https://www.ruby-lang.org/en/news/2015/03/06/google-summer-of-code-2015
      * https://github.com/railsgsoc/ideas/wiki/2015-Ideas
      * https://rubyonrails.org/2015/3/4/google-summer-of-code-2015
    * 2014
      * http://sciruby.com/blog/2014/02/24/gsoc-2014/

---

## BOOKS
 * 2021 [Bug Bounty Hunting for Web Security](https://github.com/jasnow/bug-hunting-web-security) book
 * 2020 [Black Hat Ruby](https://github.com/blackhatruby/BHR_Labs) book's code
 * 2009 [Security on Rails](TBD) book's code.

---
## REPOS - Ruby-related Security projects
 * [metasploit](https://metasploit.com)
   * https://summerofcode.withgoogle.com/archive/2023/organizations/metasploit
 * [Railsgoat](https://github.com/OWASP/railsgoat)
   * 2018: https://github.com/OWASP/www-community/blob/master/pages/
     initiatives/gsoc/gsoc2018ideas.md
 * [Ronin](https://ronin-rb.dev): Security Toolkit
 * [ruby-advisory-db](https://github.com/rubysec/ruby-advisory-db) (used by
   "bundle audit")

## VULNERABLITY RESOURCES
 * [vulnerablecode](https://github.com/aboutcode-org/vulnerablecode) - Database of open source software package vulnerabilities.
 * [vuln-list-update](https://github.com/aquasecurity/vuln-list-update) - Collects vulnerability information and saves it in parsable format automatically.

## REPOS WITH VULNERABILITIES (See more at bottom of this file)
 1. rails_new 
 2. Public "railsgoat"
 3. DVGM
 4. rails_sql_injection
 5. vulnerableApp
 6. damn_vulnerable_rails_app
 7. spxxrt_2_3
 8. oct11

---
## Al's Definition of "Vulnerable" Repo
 * 12/27/2025: COMMANDS
   * https://owasp.slack.com
   * Run "rake".
   * Run "brakeman".
   * Run "bundle-audit".
   * Run "ruby_audit". (1/2/2026: dropped)

---
## Definition Applied on 12/28/2025:
 1. rails_new (41)
    * "rake" (GitHub found 41 vulnerabilities on jasnow/rails_new's
       default branch (6 critical, 11 high, 13 moderate, 11 low).
       * "bundle audit" (none)
       * brakeman/Security Warnings: ZERO

 2. Public "railsgoat" - https://github.com/OWASP/railsgoat (18)
    * (rg25) RAILSGOAT_MAINTAINER="yes" rake
    * bundle audit (none)
    * brakeman/Security Warnings: 18
      * Command Injection: 1
      * Cross-Site Request Forgery: 1
      * Cross-Site Scripting: 2
      * Dangerous Send: 1
      * File Access: 1
      * Format Validation: 1
      * Mass Assignment: 2
      *- Redirect: 1
      * Remote Code Execution: 4
      * SQL Injection: 2
      * Session Setting: 2

 3. DVGM (7)
    * "rake" (No GH vulnerabilities)
    * "bundle audit" (none)
    * brakeman/Security Warnings: 7
      * Cross-Site Request Forgery: 1
      * Cross-Site Scripting: 2
      * Mass Assignment: 1
      * SQL Injection: 3

 4. rails_sql_injection  (3)
    * "rake" (No GH vulnerabilities)
    * "bundle audit" (none)
    * brakeman/Security Warnings: 3
      * SQL Injection: 2
      * Session Setting: 1

 5. vulnerableApp (2)
    * "rake" (No GH vulnerabilities)
    * "bundle audit" (none)
    * brakeman/Security Warnings: 2
      * Dynamic Render Path: 2

 6. damn_vulnerable_rails_app (1)
    * "rake" (No GH vulnerabilities)
    * "bundle audit" (none)
    * brakeman/Security Warnings: 1
      * SQL Injection: 1

 7. spxxrt_2_3 (1)
    * "rake" (1)
      * https://github.com/jasnow/spxxrt_2_3/security/dependabot/33 (Trix)	   
    * "bundle audit" (none)
    * brakeman/Security Warnings (none)

 8. oct11 (1)
    * "rake" (1)
       * https://github.com/jasnow/oct10/security/dependabot/29
    * "bundle audit" (none)
    * brakeman/Security Warnings (none)
EOF
