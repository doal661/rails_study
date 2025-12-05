## 🚧 Project Context: Engineering Under Extreme Constraints

> *This section was added retrospectively to document the specific engineering challenges overcome during development.*



**Critical Hardware Instability (Disaster Recovery)**

Developed on a **depreciated classroom desktop** with severe hardware degradation (Disk I/O errors).

* **Challenge:** Encountered critical boot failures (**GRUB rescue mode** & **Early-stage Kernel Panic**) approximately **once a week**.

* **Response:** Established a routine **recovery process** involving full OS (CentOS 7) re-installation and environment provisioning to ensure project continuity.



**Network & Environment Constraints**

* **Network:** Overcame the lack of static IP by implementing **DuckDNS** and **configuring server binding with the domain** to enable mobile testing on the local network.

* **Dependency:** Resolved version conflicts between **Ruby**, **Rails 7**, and **Legacy SQLite (3.7)** through log-based troubleshooting.

-----

# README

## My hope for this article
I'm still a student, so I want a lot of feedback.
If you have improvements, please post them to the non-main brunch

-----

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby on Rails version in this project / refer to gemfile
*gem "rails"
~> 7.0.4", ">= 7.0.4.3" (X)
-> 7.0.5
* Ruby version
ruby 3.0.6p216 (2023-03-30 revision 23a532679b) [x86_64-linux] (X)
-> ruby 3.0.0p0 (2020-12-25 revision 95aff21468) [x86_64-Linux] (O)

* System dependencies
CentOS 7

* Configuration

* Database version
sqlite 3.7.17 (2013-05-20 00:56:22 118a3b35693b134d56ebd780123b7fd6f1497668)

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
=======
# rails_study
>>>>>>> 5ba6cc0a428197ba16fdcb7ff3eca53d983e98d9

## purpose of this repository
A backup of a web services project I did for a college class.
Only I used Ruby on Rails, while everyone else did it in PHP.

## If you clone my project..
-> bundle install
-> bin/rails db:migrate

## If you want to use a domain on this server
rails s -p [port_number] -b [domain_name]
example -> rails s -p 80 -b rollersm.duckdns.org

## If you have a lower version of Ruby
You will need to modify the .ruby-version and the ruby in the gemfile.
