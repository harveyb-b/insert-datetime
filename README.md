                long unixTimeStamp = Convert.ToInt64(data["list"][i]["dt"]);
                DateTime dateTime = DateTimeOffset.FromUnixTimeSeconds(unixTimeStamp).DateTime;
                dataGridView1.Rows[0].Cells[i].Value = dateTime.ToString("ddd, dd MMM");
                
                for (int i = 0; i < 24; i++)
            {
            
            
            }
                
                
                double temperature = Convert.ToDouble(data["list"][i]["main"]["temp"]);
                dataGridView1.Rows[2].Cells[i].Value = $"{temperature}°C";
