# AR_v.3.3.3
public DataTable ReadDataTable()
        {
            var orec = new DbfRecord(this.Header);
            var orec = new DbfRecord(Header);
            DataTable dataTable = new DataTable();
            foreach (var column in this.Header.Columns)
            foreach (var column in Header.Columns)
                dataTable.Columns.Add(column.Name, column.ColumnBaseType);
            while (ReadNext(orec))
