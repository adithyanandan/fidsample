# fidsample
import java.util.List;

public class Payload {
    private List<Data> data;

    public List<Data> getData() {
        return data;
    }

    public void setData(List<Data> data) {
        this.data = data;
    }

    public static class Data {
        private String contentId;
        private String population;
        private String reminderFlag;

        public String getContentId() {
            return contentId;
        }

        public void setContentId(String contentId) {
            this.contentId = contentId;
        }

        public String getPopulation() {
            return population;
        }

        public void setPopulation(String population) {
            this.population = population;
        }

        public String getReminderFlag() {
            return reminderFlag;
        }

        public void setReminderFlag(String reminderFlag) {
            this.reminderFlag = reminderFlag;
        }
    }
}
import com.fasterxml.jackson.core.JsonProcessingException;
import com.fasterxml.jackson.databind.ObjectMapper;

public class Main {
    public static void main(String[] args) {
        // Create the object
        Payload payload = new Payload();
        Payload.Data data = new Payload.Data();
        data.setContentId("Test_Email");
        data.setPopulation("Dynamic");
        data.setReminderFlag("N");

        // Add the data to the list in payload
        payload.getData().add(data);

        // Convert the object to JSON
        ObjectMapper objectMapper = new ObjectMapper();
        String jsonPayload;
        try {
            jsonPayload = objectMapper.writeValueAsString(payload);
            // Print or send jsonPayload to the front end
            System.out.println(jsonPayload);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
        }
    }
}



 "contentIdLists": [
            {
                "entries": [
                    {
                        "contentId": "Test_Email",
                        "population": "Dynamic",
                        "reminderFlag": "N"
                    },
                    {
                       
                      "contentId": "Test_Email",
                        "population": "Dynamic",
                        "reminderFlag": "N"
                    }
                     ]
            }
        ]![image](https://github.com/adithyanandan/fidsample/assets/28766388/2e0467c5-e3e5-4101-90f2-9417243e37c0


        $scope.contentIdLists = [
          {
            entries: [
              {
                contentId: "Test_Email",
                population: "Dynamic",
                reminderFlag: "N"
              },
              {
                contentId: "Test_Email_2",
                population: "Dynamic",
                reminderFlag: "N"
              }
            ]
          }
        ];

        "<jqx-combo-box id='populateEx' ng-disabled=\"$ctrl.disabledFields\" remove-model ng-model=\"$ctrl.populationOptEx\" ng-disabled=' $ctrl.disabledFields'" +
			"jqx-settings=\"populationSettingsEx\" jqx-on-close=\"changeHandler_POPULATIONINDEx(event)\" style=\"margin-top: 5px;\" spark-change-data></jqx-combo-box>" +

			"</div>" +
			"<div class=\"col-sm-1 deleteIcon\">" +
			"<a href=\"\" ng-disabled=\"$ctrl.disabledFields\"ng-class=\"{disabled: $ctrl.disabledFields}\" ng-click=\"$ctrl.deleteComponentEx($event,'populationOptEx',5)\"> <span class=\"glyphicon glyphicon-trash\"></span></a>" +
			"</div>";
