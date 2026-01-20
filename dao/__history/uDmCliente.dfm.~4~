object DmCliente: TDmCliente
  Height = 575
  Width = 804
  PixelsPerInch = 120
  object sqlPesquisar: TSQLDataSet
    CommandText = 
      'SELECT id, nome, telefone'#13#10'FROM NEW_TABLE'#13#10'WHERE (nome LIKE :nom' +
      'e)'
    MaxBlobSize = -1
    Params = <
      item
        DataType = ftString
        Name = 'nome'
        ParamType = ptInput
      end>
    SQLConnection = DmConexao.sqlConexao
    Left = 32
    Top = 48
  end
  object sqlInserir: TSQLDataSet
    CommandText = 
      'insert into new_table (id, nome, tipo, documento, telefone)'#13#10'val' +
      'ues (:id, :nome, :tipo, :documento, :telefone)'
    MaxBlobSize = -1
    Params = <
      item
        DataType = ftInteger
        Name = 'id'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'nome'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'tipo'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'documento'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'telefone'
        ParamType = ptInput
      end>
    SQLConnection = DmConexao.sqlConexao
    Left = 152
    Top = 48
  end
  object sqlAlterar: TSQLDataSet
    CommandText = 
      'update new_table'#13#10'set nome = :nome,'#13#10'    tipo = :tipo,'#13#10'    docu' +
      'mento = :documento,'#13#10'    telefone = :telefone'#13#10'where (id = :id)'
    MaxBlobSize = -1
    Params = <
      item
        DataType = ftString
        Name = 'nome'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'tipo'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'documento'
        ParamType = ptInput
      end
      item
        DataType = ftString
        Name = 'telefone'
        ParamType = ptInput
      end
      item
        DataType = ftInteger
        Name = 'id'
        ParamType = ptInput
      end>
    SQLConnection = DmConexao.sqlConexao
    Left = 264
    Top = 48
  end
  object sqlExcluir: TSQLDataSet
    CommandText = 'delete from new_table'#13#10'where (id = :id)'
    MaxBlobSize = -1
    Params = <
      item
        DataType = ftInteger
        Name = 'id'
        ParamType = ptInput
      end>
    SQLConnection = DmConexao.sqlConexao
    Left = 368
    Top = 48
  end
  object dspPesquisar: TDataSetProvider
    DataSet = sqlPesquisar
    Left = 32
    Top = 136
  end
  object cdsPesquisar: TClientDataSet
    Aggregates = <>
    Params = <
      item
        DataType = ftString
        Name = 'nome'
        ParamType = ptInput
      end>
    ProviderName = 'dspPesquisar'
    Left = 32
    Top = 224
    object cdsPesquisarID: TIntegerField
      FieldName = 'ID'
      Required = True
    end
    object cdsPesquisarNOME: TStringField
      FieldName = 'NOME'
      Required = True
      Size = 80
    end
    object cdsPesquisarTELEFONE: TStringField
      FieldName = 'TELEFONE'
      Size = 10
    end
  end
end
