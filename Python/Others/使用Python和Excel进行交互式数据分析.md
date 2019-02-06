ԭ�ģ�[Interactive Data Analysis with Python and Excel](http://pbpython.com/xlwings-pandas-excel.html)

---

      ![article header image](http://pbpython.com/images/article-overview.png)

## ���

���Ѿ�д��[�ü�](http://pbpython.com/improve-pandas-excel-output.html) [��](http://pbpython.com/advanced-excel-workbooks.html)����[pandas](http://pandas.pydata.org/)��Ϊһ�����ݲ���/��Ƥ���ߣ��Լ���������ܹ���Ч�ش�Excel��ȡ��д�����ݣ��Ƕ�ô�ĺ��á����ǣ�����Щ����ҪΪ���ݷ����ṩһ������ʽ����������£���ͼ�ڴ�Python�У���һ���û��Ѻõķ�ʽ�������ϵ�һ�𣬽������ѵġ���ƪ���½����������ʹ��[xlwings](http://xlwings.org/)����Excel, Python��pandas����һ���Թ���һ�����ݷ������ߣ�������ߴ�һ���ⲿ�����ݿ�����ȡ��Ϣ����������������һ����Ϥ�ĵ��ӱ���ʽ������ָ��û���


## һ�����ٵ�Excel�Զ������

Excelʹ��VBA֧��һЩ�Զ���ѡ��û����庯��(UDF��User Defined Functions)���൱�򵥵ģ����ǽ������룬Ȼ�󷵻�һ���򵥵�ֵ����ǿ���ѡ����һ���꣨����̣������ǿ����Զ���ɼ����κ�Excel�����������¡�

����UDF�ͺ���ǿ��ģ�����������Ȼ����VBAд�ģ�����ʱ�򣬽�Python�������������ǻ���Excel�Ľ��������ǳ����á������xlwings������֮�ء���򵥵�˵��xlwings����������������Ҫ��ʽճ��python��Excel��

*   ��Python�п���Excel
*   ��Excel�е����Զ����Python����

���Ľ��ص㹹��һ���������Զ����Python�����Excel������


## �����ǡ���

����������У����ǽ�����һ���򵥵Ľ�ģӦ�ã���������ĳ������һ���˺��Լ����ڷ�Χ��Ȼ�󷵻�һЩ�Ѿ�ͨ��pandasת�����ܽ��������Ϣ����������Ǽ򵥵ģ�������ʾ�����ֽ�ϵ��������Լ�ִ��һЩ�����ӵ����ݷ����ж�ô�򵥡�

������һ������������ͼ���������ͼ��

![data flow](http://pbpython.com/images/python-data-flow.png)

��������ӿ��Ժ����׵���չ����ѯ������ݿ⣬�������κ�Python���Զ�ȡ���ļ�(CSV, Excel, json�ȵ�)���н�����


## ��װ����

Ϊ�˴ﵽ��ƪ���µ�Ŀ�ģ��ҽ���������һ������Windows��ϵͳ�����и�Ӧ�á���ǿ�ҽ�����ʹ��[anaconda](https://www.continuum.io/downloads) (����[miniconda](http://conda.pydata.org/miniconda.html))��Ϊ��ѡ��ķ��а汾��

������Ҫ���ĵ�һ�����ǰ�װxlwings������python+pandas�Ѿ���װ���ˣ���
```sh
conda install xlwings
```

>�汾����
>xlwings�ڲ��ϵĸ����С��������ʱ����0.7.1�汾�ġ�

��һ��Ư������Ϊ`quickstart`��xlwings��������������Ϊ�㴴��һ��Excel�ļ�������Python�ļ�׮��
```sh
c:\>xlwings quickstart pbp_proj
```

����㿴һ���´�����pbp_projĿ¼����ô�㽫���������ļ���
```
pbp_proj.py
pbp_proj.xlsm
```

���У�Python�ļ��ǿյģ���Excel����ȥҲ�ǿյģ����ǣ�Ļ���Ѿ������һЩ��������ʹ��excel��Python�ӿڸ������ס�

Ҫ����Excel�ļ�����ɶ������Excel�д����´������ļ���Ȼ��ѡ��Developer -> Visual Basic��Ȼ����Ӧ�ÿ��Կ���һЩ�������Ķ�����

![vba setup](http://pbpython.com/images/excel-vba-setup.png)

��ᷢ��������ģ�� - `xlwings`��`Module1`��xlwingsģ��������е�VBA���룬�Ӷ�ʹ�����Զ���Ĵ�����á��ڴ��������£���Ӧ�ò�Ҫ������Ȼ��������������������(�����޷��ҵ�Python)����ô��������������������Ϣ��

![config](http://pbpython.com/images/excel-config.png)

`Module1`����һЩĬ�ϴ��룬���ǿ������������ģ�

![sample module](http://pbpython.com/images/excel-sample-call.png)

һ�ᣬ���ǽ��޸��������������Զ���Ĵ��롣���ȣ�����Ҫ����Excel�����ļ���

�������Ӧ�ã����ǽ������û�����һ���˺ţ���ʼ���ںͽ������ڣ�Ȼ�󽫻�����Щ��������������ڡ�

�����Ǽ򵥵ĵ��ӱ��

![simple spreadsheet](http://pbpython.com/images/excel-base.png)

��ֻ������һЩС�ĸ�ʽ�޸ģ���Щ�����в�û�й�ʽ������ؽ��޸ı��浽Excel�ļ��С�

��һ�����ҽ�����һ����̵�Python��������˵������δ�Excel�ж�ȡ���ݣ�Ȼ������д�ص�Excel�С��ҽ���������һ����Ϊ`pbp_proj.py`�Ŀ��ļ��С�
```py
import pandas as pd
from xlwings import Workbook, Range


def summarize_sales():
    """
    Retrieve the account number and date ranges from the Excel sheet
    """
    # Make a connection to the calling Excel file
    wb = Workbook.caller()

    # Retrieve the account number and dates
    account = Range('B2').value
    start_date = Range('D2').value
    end_date = Range('F2').value

    # Output the data just to make sure it all works
    Range('A5').value = account
    Range('A6').value = start_date
    Range('A7').value = end_date
```

�ó����Ǽ򵥵ģ������ڻ�ûɶ�á����룬Ϊ��ȷ�����еġ��ܵ������͸�λ������һ����ܳ��������Щ��Ҫ��ס�Ĺؼ�һ���ǣ�����ļ���Ϊ`pbp_proj.py`����������Ϊ`summarize_sales`��

Ҫ����һ��д��һ��������Ҫ����һ��Excel�������������ǵĴ��룺

![simple spreadsheet](http://pbpython.com/images/excel-run-code.png)

����ʱ�൱���ģ���ֻ�ǵ����ģ�飬Ȼ��ִ�к�����
```
Sub RetrieveSales()
    RunPython ("import pbp_proj;pbp_proj.summarize_sales()")
End Sub
```

���һ�������һ����ť�����ǵı��У�Ȼ������������/��`RetrieveSales`��

![assign the macro](http://pbpython.com/images/assign-macro.png)

һ���������������Ӧ�ÿ��԰��°�ť��Ȼ�󿴵��������Ķ�����

![simple example](http://pbpython.com/images/simple-demo.png)

���������Ѿ����ˣ����ǿ��Դ�Excel��ȡ��Python�����У�Ȼ��ʹ�ö�ȡ��������������ݵ�Excel�����ڣ�������ʹ�������Щ��


## �����ݿ��ж�ȡ����

����������У��ҽ�ʹ��[sqlalchemy](http://www.sqlalchemy.org/)����ѯһ��С��sqlite db��Ȼ��ֱ�ӽ���ȡ��ѯ��һ��pandas dataframe�С����ַ����ĺô��ǣ���������Ҫ��ѯ��һ�����ݿ⣬��ô�����ֻ���޸�slqlalchemy���棬Ȼ�󱣳���Ĵ����ʣ�ಿ�ֲ��䡣��Ϊ�ο���xlwings��վ��������һ��[����](http://xlwings.org/examples/)����Ϊ��һ���Ĳο����������Ӧ�ú��а�����

�ڴ������֮ǰ��ȷ����װ��sqlalchemy��
```py
conda install sqlalchemy
```

���������ͨ��ʹ�õ����ݿ������·�������ӵ���sqlite���棺
```py
from sqlalchemy import create_engine

# Connect to sqlite db
db_file = os.path.join(os.path.dirname(wb.fullname), 'pbp_proj.db')
engine = create_engine(r"sqlite:///{}".format(db_file))
```

���ڣ������������ˣ����ǿ��Թ�����ִ�в�ѯ��Ȼ�󽫽����ȡ��һ��dataframe�У�
```py
# Create SQL query
sql = 'SELECT * from sales WHERE account="{}" AND date BETWEEN "{}" AND "{}"'.format(account, start_date, end_date)

# Read query directly into a dataframe
sales_data = pd.read_sql(sql, engine)
```

һ�����ǽ����ݱ�����`sales_data` dataframe�У����ǿ������κ��������������顣Ϊ�˼��������һ���һ���򵥵�`groupby`��Ȼ������֧����`sum`��
```py
# Analyze the data however we want
summary = sales_data.groupby(["sku"])["quantity", "ext-price"].sum()
total_sales = sales_data["ext-price"].sum()
```

���˵��ǣ�xlwings����⡱pandas dataframe����˽�ֵ���ص�Excel�������кܼ򵥣�
```py
Range('A5').value = summary
Range('E5').value = "Total Sales"
Range('F5').value = total_sales
```

�������������Excel -> Python -> Excel��������

### �����ĳ���

�����ǰ�����`pbp_proj.py`�е�ȫ���ܴ��룺
```py
import pandas as pd
from sqlalchemy import create_engine
from xlwings import Workbook, Range
import os


def summarize_sales():
    """
    Retrieve the account number and date ranges from the Excel sheet
    Read in the data from the sqlite database, then manipulate and return it to excel
    """
    # Make a connection to the calling Excel file
    wb = Workbook.caller()

    # Connect to sqlite db
    db_file = os.path.join(os.path.dirname(wb.fullname), 'pbp_proj.db')
    engine = create_engine(r"sqlite:///{}".format(db_file))

    # Retrieve the account number from the excel sheet as an int
    account = Range('B2').options(numbers=int).value

    # Get our dates - in real life would need to do some error checking to ensure
    # the correct format
    start_date = Range('D2').value
    end_date = Range('F2').value

    # Clear existing data
    Range('A5:F100').clear_contents()

    # Create SQL query
    sql = 'SELECT * from sales WHERE account="{}" AND date BETWEEN "{}" AND "{}"'.format(account, start_date, end_date)

    # Read query directly into a dataframe
    sales_data = pd.read_sql(sql, engine)

    # Analyze the data however we want
    summary = sales_data.groupby(["sku"])["quantity", "ext-price"].sum()

    total_sales = sales_data["ext-price"].sum()

    # Output the results
    if summary.empty:
        Range('A5').value = "No Data for account {}".format(account)
    else:
        Range('A5').options(index=True).value = summary
        Range('E5').value = "Total Sales"
        Range('F5').value = total_sales
```

�����ǽ��������

![full example](http://pbpython.com/images/final-result.png)

All of the data, including the sqlite db is in my github ���е����ݣ�����sqlite db�������ҵ�github [repo](https://github.com/chris1610/pbpython/tree/master/code/pbp_proj)��


### �ܽ�

xlwings�ṩ�˴�Python��Excel�޷콻����һ�����õĹ��ܡ�ͨ��ʹ�ô˴��룬�����Ϊ���Լ�����Щ�Ӷ��Դ��ȡ���ݣ������ڷǳ���Ϥ��Excel�����з������ݵķǼ����û������ɹ�������ʽ���ߡ�һ���������˽ṹ����ô�����и��ӵ��߼������ݷ����ŵ�Python�ļ��У�������������Python��̬ϵͳ���ṩ�Ĺ��ߣ��⽫�Ƿǳ����õġ���ϣ����һ���㿪ʼ���������ô��ᷢ���кܶ������ʹ�����������Python��������������һЩ����ʹ��Excel��Ϊ����Ψһ�����ݷ������ߵķǼ����û���
