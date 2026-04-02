#for changing done to pending in sql

#1.--Remove the existing column //dont run
#ALTER TABLE pumppatrol.telegram_log
#DROP COLUMN processing_status;

#-- 2. Add it back fresh (defaults all rows to 'Pending')//dont run
#ALTER TABLE pumppatrol.telegram_log
#ADD COLUMN processing_status ENUM('Pending', 'Done') DEFAULT 'Pending';

to clear signal_master table
TRUNCATE TABLE pumppatrol.signal_master;