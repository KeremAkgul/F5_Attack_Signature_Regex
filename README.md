# F5_Attack_Signature_Regex

mysql -uroot -p`perl -I/ts/packages -MPassCrypt -nle 'print PassCrypt::decrypt_password($_)' /var/db/mysqlpw` -e "select * from PLC.NEGSIG_SIGNATURES;" >> /var/tmp/attack-sigs-descrption.csv

This script will generate CSV file that includes all Attack Signature Information. Column names is as below, replace * from mysql query to necessary column names;

sig_id
rev	
flg_is_user_defined	sig_name
rule
last_update	apply_to
attack_type_id	risk
accuracy
sig_desc
last_enforcement_change	threshold_in_seconds
buffer_type_mask
flg_has_valuecontent_http
flg_has_valuecontent_xml
flg_is_hidden
flg_has_valuecontent_json
flg_has_valuecontent_gwt
flg_has_headercontent
flg_has_uricontent
flg_has_requestcontent
rest_uuid
flg_has_valuecontent_plain_text
flg_has_responsecontent
flg_has_cve
