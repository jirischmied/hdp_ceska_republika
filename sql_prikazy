-- SQL příkazy pro zpracování dat od Světové banky
-- spuštěno v SQL Server Management Studio 19
-- "GDP (current US$)" je naimportováno jako tabulka "HDP_nominalni" - konkrétně soubor API_NY.GDP.MKTP.CD_DS2_en_csv_v2_5728855.csv
-- "GDP (constant 2015 US$)" je naimportováno jako tabulka "HDP_realne" - konkrétně soubor API_NY.GDP.MKTP.KD_DS2_en_csv_v2_5728927.csv


-- zpracování dat nominálního HDP:
ALTER TABLE HDP_nominalni
DROP COLUMN column3, column4, column68

DELETE FROM HDP_nominalni
WHERE column1 = 'Country Name'

SELECT *
INTO #HDP_nominalni_CZE
FROM HDP_nominalni
WHERE column2 = 'CZE'

EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column1' , 'Zeme' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column2' , 'Kod_zeme' , 'COLUMN'

EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column5' , 'Rok_1960' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column6' , 'Rok_1961' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column7' , 'Rok_1962' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column8' , 'Rok_1963' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column9' , 'Rok_1964' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column10' , 'Rok_1965' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column11' , 'Rok_1966' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column12' , 'Rok_1967' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column13' , 'Rok_1968' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column14' , 'Rok_1969' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column15' , 'Rok_1970' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column16' , 'Rok_1971' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column17' , 'Rok_1972' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column18' , 'Rok_1973' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column19' , 'Rok_1974' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column20' , 'Rok_1975' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column21' , 'Rok_1976' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column22' , 'Rok_1977' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column23' , 'Rok_1978' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column24' , 'Rok_1979' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column25' , 'Rok_1980' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column26' , 'Rok_1981' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column27' , 'Rok_1982' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column28' , 'Rok_1983' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column29' , 'Rok_1984' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column30' , 'Rok_1985' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column31' , 'Rok_1986' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column32' , 'Rok_1987' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column33' , 'Rok_1988' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column34' , 'Rok_1989' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column35' , 'Rok_1990' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column36' , 'Rok_1991' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column37' , 'Rok_1992' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column38' , 'Rok_1993' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column39' , 'Rok_1994' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column40' , 'Rok_1995' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column41' , 'Rok_1996' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column42' , 'Rok_1997' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column43' , 'Rok_1998' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column44' , 'Rok_1999' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column45' , 'Rok_2000' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column46' , 'Rok_2001' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column47' , 'Rok_2002' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column48' , 'Rok_2003' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column49' , 'Rok_2004' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column50' , 'Rok_2005' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column51' , 'Rok_2006' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column52' , 'Rok_2007' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column53' , 'Rok_2008' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column54' , 'Rok_2009' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column55' , 'Rok_2010' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column56' , 'Rok_2011' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column57' , 'Rok_2012' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column58' , 'Rok_2013' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column59' , 'Rok_2014' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column60' , 'Rok_2015' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column61' , 'Rok_2016' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column62' , 'Rok_2017' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column63' , 'Rok_2018' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column64' , 'Rok_2019' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column65' , 'Rok_2020' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column66' , 'Rok_2021' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_nominalni_CZE.column67' , 'Rok_2022' , 'COLUMN'

SELECT Zeme, Kod_zeme, Rok, HDP_nominalni
INTO HDP_nominalni_CZE
FROM
(SELECT Zeme, Kod_zeme, Rok_1960, Rok_1961, Rok_1962, Rok_1963, Rok_1964, Rok_1965, Rok_1966, Rok_1967, Rok_1968, Rok_1969, Rok_1970, Rok_1971, Rok_1972, Rok_1973, Rok_1974, Rok_1975, Rok_1976, Rok_1977, Rok_1978, Rok_1979, Rok_1980, Rok_1981, Rok_1982, Rok_1983, Rok_1984, Rok_1985, Rok_1986, Rok_1987, Rok_1988, Rok_1989, Rok_1990, Rok_1991, Rok_1992, Rok_1993, Rok_1994, Rok_1995, Rok_1996, Rok_1997, Rok_1998, Rok_1999, Rok_2000, Rok_2001, Rok_2002, Rok_2003, Rok_2004, Rok_2005, Rok_2006, Rok_2007, Rok_2008, Rok_2009, Rok_2010, Rok_2011, Rok_2012, Rok_2013, Rok_2014, Rok_2015, Rok_2016, Rok_2017, Rok_2018, Rok_2019, Rok_2020, Rok_2021, Rok_2022 
FROM #HDP_nominalni_CZE) AS ActualData
UNPIVOT
(
HDP_nominalni
FOR Rok IN (Rok_1960, Rok_1961, Rok_1962, Rok_1963, Rok_1964, Rok_1965, Rok_1966, Rok_1967, Rok_1968, Rok_1969, Rok_1970, Rok_1971, Rok_1972, Rok_1973, Rok_1974, Rok_1975, Rok_1976, Rok_1977, Rok_1978, Rok_1979, Rok_1980, Rok_1981, Rok_1982, Rok_1983, Rok_1984, Rok_1985, Rok_1986, Rok_1987, Rok_1988, Rok_1989, Rok_1990, Rok_1991, Rok_1992, Rok_1993, Rok_1994, Rok_1995, Rok_1996, Rok_1997, Rok_1998, Rok_1999, Rok_2000, Rok_2001, Rok_2002, Rok_2003, Rok_2004, Rok_2005, Rok_2006, Rok_2007, Rok_2008, Rok_2009, Rok_2010, Rok_2011, Rok_2012, Rok_2013, Rok_2014, Rok_2015, Rok_2016, Rok_2017, Rok_2018, Rok_2019, Rok_2020, Rok_2021, Rok_2022)
) AS UnpivotData

-- zpracování dat reálného HDP:
ALTER TABLE HDP_realne
DROP COLUMN column3, column4, column68

DELETE FROM HDP_realne
WHERE column1 = 'Country Name'

SELECT *
INTO #HDP_realne_CZE
FROM HDP_realne
WHERE column2 = 'CZE'

EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column1' , 'Zeme' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column2' , 'Kod_zeme' , 'COLUMN'

EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column5' , 'Rok_1960' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column6' , 'Rok_1961' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column7' , 'Rok_1962' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column8' , 'Rok_1963' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column9' , 'Rok_1964' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column10' , 'Rok_1965' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column11' , 'Rok_1966' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column12' , 'Rok_1967' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column13' , 'Rok_1968' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column14' , 'Rok_1969' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column15' , 'Rok_1970' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column16' , 'Rok_1971' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column17' , 'Rok_1972' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column18' , 'Rok_1973' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column19' , 'Rok_1974' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column20' , 'Rok_1975' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column21' , 'Rok_1976' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column22' , 'Rok_1977' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column23' , 'Rok_1978' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column24' , 'Rok_1979' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column25' , 'Rok_1980' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column26' , 'Rok_1981' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column27' , 'Rok_1982' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column28' , 'Rok_1983' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column29' , 'Rok_1984' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column30' , 'Rok_1985' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column31' , 'Rok_1986' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column32' , 'Rok_1987' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column33' , 'Rok_1988' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column34' , 'Rok_1989' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column35' , 'Rok_1990' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column36' , 'Rok_1991' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column37' , 'Rok_1992' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column38' , 'Rok_1993' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column39' , 'Rok_1994' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column40' , 'Rok_1995' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column41' , 'Rok_1996' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column42' , 'Rok_1997' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column43' , 'Rok_1998' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column44' , 'Rok_1999' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column45' , 'Rok_2000' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column46' , 'Rok_2001' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column47' , 'Rok_2002' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column48' , 'Rok_2003' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column49' , 'Rok_2004' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column50' , 'Rok_2005' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column51' , 'Rok_2006' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column52' , 'Rok_2007' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column53' , 'Rok_2008' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column54' , 'Rok_2009' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column55' , 'Rok_2010' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column56' , 'Rok_2011' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column57' , 'Rok_2012' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column58' , 'Rok_2013' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column59' , 'Rok_2014' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column60' , 'Rok_2015' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column61' , 'Rok_2016' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column62' , 'Rok_2017' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column63' , 'Rok_2018' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column64' , 'Rok_2019' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column65' , 'Rok_2020' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column66' , 'Rok_2021' , 'COLUMN'
EXEC tempdb.sys.sp_rename '#HDP_realne_CZE.column67' , 'Rok_2022' , 'COLUMN'

SELECT Zeme, Kod_zeme, Rok, HDP_realne
INTO HDP_realne_CZE
FROM
(SELECT Zeme, Kod_zeme, Rok_1960, Rok_1961, Rok_1962, Rok_1963, Rok_1964, Rok_1965, Rok_1966, Rok_1967, Rok_1968, Rok_1969, Rok_1970, Rok_1971, Rok_1972, Rok_1973, Rok_1974, Rok_1975, Rok_1976, Rok_1977, Rok_1978, Rok_1979, Rok_1980, Rok_1981, Rok_1982, Rok_1983, Rok_1984, Rok_1985, Rok_1986, Rok_1987, Rok_1988, Rok_1989, Rok_1990, Rok_1991, Rok_1992, Rok_1993, Rok_1994, Rok_1995, Rok_1996, Rok_1997, Rok_1998, Rok_1999, Rok_2000, Rok_2001, Rok_2002, Rok_2003, Rok_2004, Rok_2005, Rok_2006, Rok_2007, Rok_2008, Rok_2009, Rok_2010, Rok_2011, Rok_2012, Rok_2013, Rok_2014, Rok_2015, Rok_2016, Rok_2017, Rok_2018, Rok_2019, Rok_2020, Rok_2021, Rok_2022 
FROM #HDP_realne_CZE) AS ActualData
UNPIVOT
(
HDP_realne
FOR Rok IN (Rok_1960, Rok_1961, Rok_1962, Rok_1963, Rok_1964, Rok_1965, Rok_1966, Rok_1967, Rok_1968, Rok_1969, Rok_1970, Rok_1971, Rok_1972, Rok_1973, Rok_1974, Rok_1975, Rok_1976, Rok_1977, Rok_1978, Rok_1979, Rok_1980, Rok_1981, Rok_1982, Rok_1983, Rok_1984, Rok_1985, Rok_1986, Rok_1987, Rok_1988, Rok_1989, Rok_1990, Rok_1991, Rok_1992, Rok_1993, Rok_1994, Rok_1995, Rok_1996, Rok_1997, Rok_1998, Rok_1999, Rok_2000, Rok_2001, Rok_2002, Rok_2003, Rok_2004, Rok_2005, Rok_2006, Rok_2007, Rok_2008, Rok_2009, Rok_2010, Rok_2011, Rok_2012, Rok_2013, Rok_2014, Rok_2015, Rok_2016, Rok_2017, Rok_2018, Rok_2019, Rok_2020, Rok_2021, Rok_2022)
) AS UnpivotData

-- sloučení obou typů HDP do jedné tabulky
SELECT HDP_nominalni, HDP_realne, SUBSTRING(HDP_nominalni_CZE.Rok,5,4) AS Rok
INTO HDP_CZE
FROM HDP_nominalni_CZE
JOIN HDP_realne_CZE
ON HDP_nominalni_CZE.Rok = HDP_realne_CZE.Rok

--konečný výsledek:
SELECT *
FROM HDP_CZE 
